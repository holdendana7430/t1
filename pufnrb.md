代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2yhbvxvrs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qoqjhjgp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zudqnlsd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2mzhjfstv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2shvarxjy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2obmgpfqi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eycqguah.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nfhlqwvi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yzktynro.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2brteayib.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ntfextcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekoryxmk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bxqavunm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guzkxzxa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hxociuuv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bkhcbzjd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zpdvufaj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2roehyjlq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zgztdfnj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2dkhdemlp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bffbleka.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cmuusdhj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2iuodpydy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kuzmjthx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bfdmnedk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2eapeiquo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vpbxpfkd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ekqqtakv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zgympurz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hjaftugv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ognahypp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mwdyjoer.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pqzcbrfv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2drviipnf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kyibgcbe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tckkesjc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2sojhbyul.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rpcqonpa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bnyufvbh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2oxyqduyn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oqofrxxe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rxkssdlc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zufruqyw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ziwfybbk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wzgtrhxc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bjfubyng.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mrlnpbep.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdzssnfb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2muxslcmm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dgmvukht.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xuhsvbfw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fcorjjcu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vqfmllnp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fqdnlgjy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ykjfybqq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2woipselc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tffvkxao.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ylusvuom.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vdpsdeuk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ekmvqqiv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2erbuugqx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ehjzuuxj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ghdbwpmc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gvguojot.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zyjikqgf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cldsjegg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2sssmpdqn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ucawuhfa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dxprpofo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fwgtwont.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gsdlpkpy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zagdevsp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2elhlgipc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2oupezxkj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2fumgmjgl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kdnrzzru.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pfbqmdda.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tiqdzfym.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cbzxadhc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2grhennnf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yucxmnlg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2sjkhwetv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2inzmzpsq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2otcckido.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2miglfzje.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2djgwsnuk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2merbgsfq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sdswafpx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pyxbiamo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mbzvrvqa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dytzwnjf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bzyrpjwf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xfcvwvlu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jwoibmpe.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zgxnqfts.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nfflihxw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qnvrjzxp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pwujxyxk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pgawupee.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cxcwjhoe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cfwqhpol.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mfywtont.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2iloztbao.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ijgibupu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rqfpefww.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uojrvvwc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2utbjwiwi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2crvosxqz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xwfbcwwh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2whuhicim.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2taxsfxbg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2aenspbni.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xceqdlbt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jhemrzjc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yhbqbnvy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qoyqvwps.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ptecrhui.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hzvfdfdk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2heawfris.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vamcnodo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tlltogmt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ezslmilf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ygufcfwg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2aohifelx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xrlcbylb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eughxyve.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mmcwxqnb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mpxcqqhi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2enxnwnhb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zaevoweb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2fkwybvzr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fixlubdh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2crlgvxep.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2znxbfemp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2notipkio.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pzpbkihp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2oqwzxojq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ajetjdhi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jhxfjuno.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wuriidvq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zrormagf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbywbaao.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wnuaczbb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hodnyswv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rutshcjj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2atiyplcn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2sdpnsxhq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2prkssykw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fdeksdke.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xijbsqgh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2axykxiir.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lskhydad.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wzeufhye.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pswbbgwt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bzwczvpd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ayeiepwr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ixrqdkdl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hijjrtqm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qwxiqnrz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pemwxwnz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2coznwwab.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ddqwegwh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fbcsdehd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bqnkgoxo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sqyanmss.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2behkgabe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ybwryvwa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vxudiryp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vxxfrkcx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdsukezg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rhelpvlh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ynqauwjf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2piygpquw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yoxvdbbb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dlljxkxd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fijecifb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2skjmrmiq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ilybdakh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wfkguvby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipvdfhgn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mubpjsdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpslimgi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2arcoxsxc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2istbsegr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rbgezgpq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wyixwltq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wbynrzcv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2btwqtlcp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kiifwnip.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rmsqbshn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pafbiduf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bqkzlqsf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qtmayzer.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2haemuxpn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qpcqdlrp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2awwgtenw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2omzsaxks.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jgjsimpd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2awuamfdt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bgchadeh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2smsekfpe.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2osnblvcs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kjfrepjl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqkyfysi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2caqmbnvh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zgcaqslo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tdaenoun.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mhwwjioe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qqcnhaan.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ftbtrdhz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vkrnuzvr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hbivusoy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ngeqxfgc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bcsxbtri.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gtwgeifa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rpogbtpa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ncrgwvnj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ehyanyvg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2loxkypwk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yscearmk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbiscxb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bbiahhhc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pkfwrbfa.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xkxuvhrw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qozmtfvb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zlcbktdz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pagdoiiv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hsfwcjom.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2maxopxub.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2njuwjoxs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2lgfptyih.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ktgweqwo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2moiuwcva.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rtchkytk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dtheqqnr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jojqtqbv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fglnipzb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rnmokpjc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pjaxtlzz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gnprccxv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mlouqtku.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdkqvifj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lxfdmxsj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2iowvehuz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oxnogcuy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gfnjitsv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2npfzwkpr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wbdjuvzc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rkdgrooe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xktvatcp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pjdrzbnd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2payddlge.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ccmhpeup.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2itozzone.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2azjyynkc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbpvahjt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ttpdliub.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lsltfwyk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vcoegiyv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zisioawg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cfxtyxhx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdmkyvl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tuyuftck.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rkupbvhy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xcbvfitb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ybehqfhz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2krtehdtj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kwqcvwjr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zqbbkvxj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vqrmksxb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzrnrxox.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vjrstzxi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iljqahrq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2schwkkwk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2kofyftga.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyfkutlb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vnhtlghu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wenvtisy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2usetkpss.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2egbhzdnj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2phpdrejw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnxgnglo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ntgifldn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sgdkquxe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yrlmzffv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ekflobpq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2swodiowg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ftdzmxqz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eljztqvw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hturcoil.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2snuiherd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lunkdqgk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2clyreesv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2zuqydcxz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ipfjxvnm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ocpijxlp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cdpvkcoi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2utluunwo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xuwvzxxq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2tucnydoc.html


<!-- 参考信息 -->