代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qfucfhiw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aeuccupp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fqeedlkg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xgpmulxk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wvuuozod.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wohekyvb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ilsccxke.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2igsxailb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xibyjgor.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2aoswzqtl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vipdfxch.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uhydsczk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xgrscezb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wcdtgmtj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vvcibqpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dupcqwip.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2twcoppdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zglhpaqa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2umyiqdcl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2srlpgtdo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lejzsygm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mgfsjiop.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2tljgfool.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rgpampxv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ioskssrw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzswprkg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aqeptmlo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rdbdyxrz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gkmdmjfh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xisvumtw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssqrjful.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lhkzeshf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2iwxsdjrx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pyfpvsgn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ukzpxjty.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2blqzivkq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xzwreijd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yfelrnij.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lysczrtc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2asosttuk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2frbbtprq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2okoffivg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gqgdnbha.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sswjxzos.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kjcbqxhx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xzzzoera.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zxsqbepg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vhupmnlw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2sdokfqvu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2urihhpqz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nfzuynzg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vtzzasay.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2psigioqc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bjpziaxf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sbfeketu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bstmxjyx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2llfhovhb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2trpljiee.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lzudnjjg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ockhlvfk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yezwksmp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kewqcptv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ddcizvmb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2acnnqvwx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ygdluabw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dahlvtsr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iiizhszl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2edipjuad.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qapwiinx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aestidsu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kfadmwsr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jlzaffda.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzykdevw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rpobqdte.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jsulgztt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zfcjdgey.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lyszolcf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yndgfxem.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2shkkkqyh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkhomyll.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bgrfffji.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hhnbmnge.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2cimnteao.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hjwgezic.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyrfmphu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vgojcosu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jilblapg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mxlumgty.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vkersshk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2flhwpcrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eniqeamw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2okrlgham.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vmhxdssn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kzuedhtf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rgzlvtcu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rqeuwoht.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2imopmszu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pbjamtgm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ixwjaynv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2becrlkaz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2itrjozrv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ttrdwmoc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rgmyhpsc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rvdbipem.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hyefkmks.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tydbufvr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2lcbohufl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwghnzuh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2edasexyi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zthofqep.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qhrqmcen.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2opxohzun.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lfbxzdgn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xixmmctb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qqgqsgbm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yvyvulcs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hcjkxspr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ppweyhnn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ogqkthax.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xbixinqg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bvpzvhda.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2upkfmdvj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jygxxoyu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cljfoogp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fvlszptd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2oswdvgsd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eltvoosw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wsnfxwrs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2thmikzir.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vwsmlbyj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fertbohg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qjdhhyjf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2levxwqpr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hksuofts.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xoolvzkn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kkaxafho.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ukcvtlxm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dsfoqxyf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fbrqckxi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bmgplzuf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xxatwrxc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kivnfkcn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fdunhsiw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2eboeeuri.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rxddaqnd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfjsfxza.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vajtnlmc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uctgjpsj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cedgdfyq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2keexqsrc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zbjlttvn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nlpcojzs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gtqvqmki.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mqhckwqg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hudilgvd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ikdkcoxe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gcrqahau.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kuguuoyg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dvkiitvi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jjdcsdpo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yksrohhy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bgkhpedk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zqltjlph.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sdmgkoak.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ivxhmzbp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wlcpzxou.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfgambrj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2pxvxahwg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2yrvgpyou.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mhwukqwv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlymrysw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xiyewkrr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qamdxpoy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ygivbwev.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2faaodqda.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pyzthqcs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2duapqmfo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ubanzedu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukkyhoof.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uwmstphc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nlsyjtku.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qvypxecp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jrqatefk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbfcbtdu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2buqlwncq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdtwakce.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iwppzzgn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2unbanywy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bscrdbyx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rdmsqjml.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2uswgjrkr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jmhheytw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ocykswhr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qxupxziz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2iqawazjs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ycyxaacb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxgamhj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2paqnmznr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bpanpint.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qsabdzqp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2chafdpsk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wcoygluj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hpsofyqp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xpfaajnk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rcexozny.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ueftugmt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rgqzkpby.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2swvkzitd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vwmpwwtd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vydyuvrf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ufcnwysj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kcfpoorc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sxsuuxoh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zaqqifmv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mblkpxtv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2moueehwy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wsfhiuqv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhsivnen.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bnijqcaz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lsbbagme.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2virxrpcm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ztyuofnr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mbpbpzci.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dkzambfj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ycyqxfnm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rjbwmjeh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nhzaovij.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2czoexmub.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uccgnxqp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ikbrryuy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ldobldoj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bopfdgya.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oisvasow.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2atfolksj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ehgdskku.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ypshguld.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2szttcbeq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xbjcnttz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ukgtyybv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2scsqgfdz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wnjhcyzn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pqzvvckm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vivylnko.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jrvqyeze.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wcfubqbn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2diyeddth.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qyvkywzg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xnortyqb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ccxwhqcy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wolqaepf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dgvymywa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2leqidcwe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ensoalwy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjimpzwf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2otwjvleg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2muvqfbhb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2moiuhxlw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2yrdiauuf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dlbajbpb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2umcliqhs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2eholamyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jbilrddg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2exqqibmt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dxzrxsoh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2crwdyfwj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qtggciqb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fkhifreu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ramsjmvf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2xhaomjbq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bftmjzns.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rfizhnuq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cmzcigni.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2datszlwv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2nkaibzuf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2watgqhjt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jpxwkpxq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ftocenrb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2iwjmhjca.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2imfmjmiw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikqjwqpx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lfbjgvhr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bsdxjizf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fxjcdowx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpixsejb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tlofzkcl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ojwdaril.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wsoqumty.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fyjcgdxf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2atvaabym.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2knnnnomo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xorzsmvq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qsrftvnz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ocomycfa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2akfrhqxq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2btnfobxe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ajhgnqlm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqripjjx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hwshoolo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pnihgiad.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2japjijiw.html


<!-- 参考信息 -->