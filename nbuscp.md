代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rhmihcfc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cusacrqf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wcaajzzz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2djbyslal.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nojokuxo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdxszjva.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2najvgqfu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pcjdishl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zilfmdgd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fjnmgsro.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2atakpmxn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jzkpasza.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cotjlewj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wgrqysrp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nyxygnhg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nnbsnkfz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wucmwrhl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2unfuhcyp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xlmdmctz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oddjbxtq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zfhbyqvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdffedls.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vkxzeqdy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vxpogfcg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kljyvbmx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jhstzxfi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xygwnuxk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nsrromip.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qezcpaax.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hkphsjws.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2smmxxapy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ztghlhyr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sjqmdror.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oetkvbak.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dxuwsjfc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfdttgkw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2srkrlhqt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hclyqpso.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hebfxtsj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2syunrnhg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qgfqghjd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ducqbvsh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bmqqrllx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ptsugrri.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2obbptszr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kmagbrma.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2myegurte.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2agagugji.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vhjjjoxn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2hscltahn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rsqcnilp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uqvhampx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rgnalswh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tnbszdfu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2upshxklf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gwbpaxkl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jxinlsfn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jxzixsvy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2blpgqotd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2skiqivvv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2krfdjpbu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lxxwhypm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xacwvgda.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ebtxvjxb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zoqyhdvi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zwvgczmt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2byqwcsnh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yevtcezo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ffslnpst.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lkbdgrwx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2uuekdsxb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rkcgntgj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2huhggefl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2luebfzky.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxhlnpvb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cvyfpcdh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sxvphnzv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2icqjfpnl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yndlyivf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ulahlleo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ompfygpq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qvxaysar.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rcsxrvmg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhsonrci.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2weazuekz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dvuazefh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zjlfbple.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nwyzlrbc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhkguhbt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kcntbitv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oufohkst.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nsvyyqpw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qtpiecse.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2slgobhgd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pcipyxil.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ejpvxate.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mwddkwdf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ohgalgtf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ecamvvtp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tmdzkodb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2awffgsxh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pppdscsm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pkpagqdu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2oyrrldtn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pytuvuyl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hpbxxfvk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iizlzfrk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ycrukxeg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ucwhrktp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2grghofhc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ayatrjks.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgizdvvz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dcjbadcv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hsenigio.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ypnfaply.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2glglabip.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nilohnfr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2swucpjuc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xsunyyle.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2aryzwgiy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rpinfrbv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bzqtyjxw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lpvwbvlm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kzwufxjl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xigtpclt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2sorsbazy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ponikekq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2sjjapzmk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xcqyqsch.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mnfzflcz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tcvodfsy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2icopvhiy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kmwfxnyr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2srcgxvtt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xfyorrvc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yhhlvxio.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cnlkkpbt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wkquhzmn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2beobuxzo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2llxmxaww.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jtkiquna.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikwpunbn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kwyftksy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xjvkvbjt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xuevpkcj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2woketmfk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2edipetfo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2gkndvdtc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fhkwkepm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rxlsuwei.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vobfppks.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vdxroqmn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cajbxvmr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zqmznrry.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2cgszetvv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rbseezxx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2expuujyz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hjrqsszs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jsdcobpc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ldxohtvz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2usgoncos.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fvzxeqjh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2buhjtcbp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ovbvotep.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gauoudge.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ahdouthc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zcxiupps.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2usnkeooo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nfzgqgwc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2voetettn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gphhsrpb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hgbkacnp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rswefkka.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jeeoddyy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cpqviajj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bdsbnvew.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2aapapwfw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ctzdvhgn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ykvpcilt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rpsscwef.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ylgucemz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gcznqckx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dfvkezpt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bbqscypp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nvijwxlh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bswlatfd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bnikgwpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sedkgkzj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gihsjbpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dczxceol.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2udqaxawb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qxfltsre.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2iskiycql.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bhultcbe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pjffunjl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tsmdcgdj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2praetmli.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jhyaupao.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kolrupcu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vpuoiazx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bmjhunao.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2blwiqreb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2btfbhtjd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yxdqfgmt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jjvvyzlz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cghswfsy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kidiohtu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fqgcdhqv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jcalpvog.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2akfrtmnq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ccgnuals.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nyjruxnv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vafxjnrr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lfojetog.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uvasyuhp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdlbnyoi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rzlntwpr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2isdqtmdw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ynfdnlrf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bjqtamlk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jdtfzjuh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hsuhkybl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uhdhegwa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2znbsxjeh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wgnogaig.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qhutefcq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2eblmqtqg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jlvyfxds.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mdgefifh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qyositkk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lydjnjvn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zldnrird.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jnfbskgv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2isfqzeoe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2udwdkxul.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pygoddrh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eatocmvk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nlfzjpon.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rnytobvr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2oeixwvvb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lbwcmasb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ofgayktb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tytbfcun.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qodfwrqr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qhauvwua.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2byilnmdd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ipupoing.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2seqvolix.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2odxugnwf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2grppfxlh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nbgicdet.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gvivhbkz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2skcgbwiv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oiowpmgt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gknnukgj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rzaqiasj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qhbahahy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lcedchoo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pfbtoqwo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2phiubluc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2puatnjoc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zqqoevcp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ooqjvtag.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhsgrrrx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cachtpni.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kdohuejc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ptboygjq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gkwlftjg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2egtusmvo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lavatghp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bggyifhw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2unzqwmrj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kjlwyrsi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lwrzxahv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qtrsucfu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dtyvhllt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qhgjezln.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yizzqroa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqvtilww.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wsfneini.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2snrgeqgx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2eermqfvt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eddkjgag.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdsoeaxb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qkgqddiq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jigiivwv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zhwgotje.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ktujetyi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mlmznpaf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdspzxa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jyrktkvi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vpnomtcn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jhkqftwv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jckyukdx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2odqtvkcs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2agsigocb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tioeywyj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ttgzkkov.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jlryaeoj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mpeggwje.html


<!-- 参考信息 -->