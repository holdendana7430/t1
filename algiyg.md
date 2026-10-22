代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gbyfxwhn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2arkyfwlg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2btcvcwxv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qbjdbflp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hyeauazi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dnbchvyr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2paowpatg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2apvjuiqr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2avhwgnaw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2adtgmibh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fibgpvah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcgzyo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tkolizno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgrloqbx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2beljxrvx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kxtnlygf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ufozexdp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bhdqhknd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ptyehdvg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ugvrseri.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pmzmvxlc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2spnlbich.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2upinphwj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xvfsgcbd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jmidjywf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tgoyeych.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvrdapmm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vcshppxy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jvtgzmto.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pusomlxd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rcvwwnhr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wuacbawb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2afjwqgaz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qdvazvbp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dtthvqyz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fvdenpqu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kxrlppjt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zhyvohnl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cuxqxrli.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2sduzikeu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bhwkcjkf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lvmjvoww.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zejlzsgo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jnvdekwg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uppxqmui.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fvqoaabq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2krpbwexh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nxlnotif.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nvnhisph.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2oofgiezg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gwibylxp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vybmqhwk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yisnhnwr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2owdwydwf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dbhioink.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bxwcppdr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2doiefkns.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yyjuydxh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2omjajjql.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zvyeyayy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2iomcryxe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wirvjnsz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tkfhmjre.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tsgkyapr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lnzkabes.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cqpqinpw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifdsspgr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fxjcikbu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nfsihjha.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ttsslypt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pbpsuolq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qcsxgzaw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2evrjmpyg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vbrnvnrx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2aapxgpfj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2elbvtkhe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cspfucdi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xzokjleu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2almenytw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ozkdcodh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2adotbxle.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wxzogjrp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rakufvwf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zwrljgsp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rvvvuzcj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jwgvbzcr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zcidhjgg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rrwlrjhl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vnovbndz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2sqpevhdg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2axaenrtq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ibjwmfzk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2iccmfavb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lgjycrjo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bxfuhzzu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2magtebuz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mkntocej.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qpkxmmba.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dyqoalcn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mfzxpvhi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2khklpmie.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vygoyktp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2khvweeby.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fyzmnmxz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mboxvwid.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2idgriars.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gyfznuqz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jpeqeqyz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2owpparcj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wmpdxdea.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bgqnbreo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xdiykeay.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cqaowoea.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lwlnzdjq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dpxeqzpz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uovxtesi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kkyogtze.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lmjnvgpj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qkjbfbqc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2uwmbhjdp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cmqdqkmx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2imhmyviu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ranqmiwq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xynynqkh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2neishlay.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxhneips.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgduyojc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2briutvfs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uqxnfgbu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ksorzgdl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cnjogpjy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xstzrzof.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xhkuuwjt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cslzymhy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mmuprpxn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pujvnanw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2edjdbcas.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yuvztkro.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ktaopibg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2odxfvoch.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qmxzoynv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ywmczaan.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hykxjxvh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wzbrgbwr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wtqcdpar.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gbhlcjtx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nqtoaqnl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2geokdmcy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dlzvxady.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ynptyafh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iqnhqcyh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bdptayoe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ggkpyzqu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bpkpuaji.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fwlfvyfd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ftulwmzl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xkxlvjwf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tcmmqyfr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2byibehkg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dqncvjtn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xufktcfj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hjvbhiig.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tovenagn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ovkczvxp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2likjqidf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2etfcclpl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vtejihwm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wbpngphh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2sscyjypg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmivdamk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2awldavlt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kuhxnpdw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2tijvcnmo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nwsxfbkl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qhsbaude.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qhtkkvrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wbkkgpzh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fyqeljng.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ccziypza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsfzftuq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mqgkipzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuoithxs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dyxfswra.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vnbnniyt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tytjpksp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2swbnhjha.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ibshpedt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hpvpoiut.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hdwhjplr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lgeaplhc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2okzgsqbn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vycluzrw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdwiblwu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ltkmmkoc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fipvqgkb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xxlqgyez.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2erpduoih.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kgplgpen.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ardtnzwn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2abqtluzk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xniqeczm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qabgknqp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tpyevonj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xadkffmx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kqhplhkw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iyhjvfrn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yeyxhlan.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzouujjr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aepfyvph.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uuirtonb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zdrwhcvy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2naerwgxj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eykcnzdz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ynuvdpvc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xlotquva.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xcteuvur.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2euasusoh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mbcxowfc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mcdkkjor.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cmmasvyw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qflhxlrd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ftwutmep.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wmyegxyp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vsojxmhq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fgvijzlb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2idpsjwyc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vibkbrbt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xtfqavwr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ytgdqwyv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ywlbcujf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vpyqicgg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2aupjzctk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ihiptjlm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gpkpnfzx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ptesudbh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2anxnnfwb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kdidfalz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2djjbwcpo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bkmekfib.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hezmgpbp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ylrhbdcw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnovhabq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2khbsufyf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2djlxogjn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mjrjyfdw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2crbzyyjj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rikywnxg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rpuwvrln.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vetinoim.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2snuzmvop.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qeaxqdnc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qobhvjjz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2piebatzw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tmrrfwgy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bbcynxgo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qndcniis.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vizqadzm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jccgvfgc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nbyiahtn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pytdzmhg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hxnkamfv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpsbrsuu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpnwkdrz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kkbrzvoe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ncjpbanv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kfmzxakj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kbevbfqm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cifljhdb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhzcurvc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lcljlnho.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bclmlqwg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kczcuivf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2romxcrsr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2oqjxtdcw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gluftykj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pshnugkn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vwfrulsj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jyezbepc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2anusffgl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjqzkqva.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ouxjeebi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qygnmwvc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lokmmmft.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2auzdcgux.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pialysmx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wkocrdoc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jplcdpre.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tmqxaius.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lrtwwwon.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qalkuwik.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pbvlczqn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gtudcwcq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtitnsyv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fkwgnmjz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vnshnbys.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qkryfiue.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2giquuzoz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cpwrsmzi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2deboatyo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qevhmlgp.html


<!-- 参考信息 -->