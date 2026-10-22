代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tkkeaukj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kpxysdlr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dsafngjc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jnmsgsmo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fnawvvej.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jjfywciw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ozyhqiqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbqnxhqi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oxkebrbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbfuhufk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nxzioopb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lkmzsqqq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dsiysawt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2oxoukuqv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ighvqjmc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqmaozrk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cvlmbakw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2unlcocbb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2trpijbfa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vcaqfrim.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ygyrqpqq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ejazeyor.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dhdractn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntfwpwkp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xdfutcmi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2uegbmpyl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xgbthhyt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lauwfmrr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jgeohbrx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2stzzyczr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zwcqcdxn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fbczxzof.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2htyktwtb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fehsfyob.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lotsppfp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cvhpansd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qluhtexd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ymenvxne.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nnhofozh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zettrqpt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2stzzyjmx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gaeploou.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2znxobssr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qnqhfoxi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rjboldrh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rnmvrdnj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2eujkgrmr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mmtnkwek.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mllocgev.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lvhqfdkv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qishtpmm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uqfnsfpy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2amadmbpw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tjnloawc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhaehtma.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iiexipjx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qgelvotq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tdfhzyrh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mgwjfpaa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dtuhlqow.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kwqqovaw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hpgmgbuv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2irqzqgwb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kjwpnjkk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2txaeeqhj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zkrohgva.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2duelpuky.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2edpfhccg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2taovpvie.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2utqjnwjm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vcyddqvg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wfrlfciu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tvguhwqi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lsqssoyu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxuluh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hdrhecyo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbkwoyyh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rmhwfgxo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dqtuawtx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2aocnrdin.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uzpmklyp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hfmtjzdh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dixpdyck.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2teltbtcp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uoqdeosb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ltvkkwdp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ggrjeqyj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lwqjqhrn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2odfynasd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cgtealcp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kbgyejtj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2iblrzwyk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tuwvzejc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2egkyuboq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2oqpjjaye.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2umfnotsr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dvpietrw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2erizueta.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cmphlibv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ottomrap.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yethbdrh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2flrsppfv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uqhnejiq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2izcnfzmg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2eulzxxge.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2dopqhrnv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2glsdempc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ftzlgdvy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wjjddpat.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fvmumpns.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dksidzwc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ufmwsocg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tvkzkghd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2atxsyvkt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nkgvgcez.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zlevezun.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2gpbiimiy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cvueopwn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hgysfoyw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nauziszp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lcnqrokq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvwhdjte.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ojroysoa.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jfdnnnus.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dwjvyoxq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2akmfaikv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ncoexskz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zgmtonzm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sywzesxe.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mbxqmtqw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lnyxdlya.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sqiznxii.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dvmrkrcd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2btlvdggf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pzfyxjjf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cflramdm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gudrjljn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cvinyiij.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pnrmpfly.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vrwvaazr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2cwkwjbco.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yffodfbr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hjlzbwrj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jaugljjt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hzmjbusj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tckzhcak.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ltokyiyg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ernnshlg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lmnpvgps.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zfrtmmct.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yoeafzwq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bjfmqgkq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mlarodrn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2trgscpwh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ififcdur.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pxxgzdxi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vmvzzszh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tvcvpnbz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2owsyhcbj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ztgvqrbx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2tourruoj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ufteqldz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpqoparv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ufhfpzod.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ljabilrn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pdzvttbv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vlmhafoc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2huovwsiy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pjxlsxmd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fdowghek.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2imqsyutr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wraegvhi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vgqrqdje.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2meknadae.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vmyxzghy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sduifaua.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oipjkqnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnhlwzkx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lbxbqrye.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hlazllcf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqchmwhz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mkhaiawu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zrgpbqtt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yyspwyil.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vsauaxms.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2yputmdsz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vcdyuxlf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cazdlnnm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rdvqkjpx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zkhpvpxo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lndmtspt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2bmbayosi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mvbnqang.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2krqajawy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2scnmhxej.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2prhpenkp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2soibfgts.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dvirtkov.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jeczqzis.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eckloljv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dhvsrsbd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sqephplf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgnzsgv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2onmbjcrc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cexawagl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qoevegoi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ymkujbrl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cizulohf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dtasqtri.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bkyrrsln.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uerbchpa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zyhzydzd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdpnxvdj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bdkgdglx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2twstyajy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2frjzcmla.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zamttfdf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pyhoqsrg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mfclwuzl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2exoohvxp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xutosurx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xbsxhaph.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hzeqxjxo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pxlmkimn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qnikayoy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ymswwyqf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2osmhargw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vbofqsbx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cpheydwl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xpwlgfwh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2egsdfacc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zkltvzhl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ukzxnrma.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vglchnkr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xaacwpww.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2bvfcwede.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uzoiyket.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qdrclfdz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xesnpmwg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2favsnyin.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wyywukzg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zjgtoucu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ztndjypi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yluxzsim.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pmxavufu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vobmhtii.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fzysanvg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2shxfdcbj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ljmffdoc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zzdptkxq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wdmbdbym.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jzijhutn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vmkovrrl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fxnskhsn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fnbydnxh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jgtrqwqk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mcpeftif.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2btqkvned.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2oocwivfe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uzfgmizm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2miepujeu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oghloggo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2aeiungez.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bseycocl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcvyiwlx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zpzkitam.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2keqdcnuj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ajnfntyr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eywodwnv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2brasrici.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2csqcuync.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2scslpbne.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mjukvumi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ckcubxkg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dwjmzyjl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jaesunzj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xgkcryjt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2smhxxdpi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oygvhqdz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wzjtopbc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnlxevb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wwzqzjdv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2uvfhtsqa.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2osnngstk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cgahoaln.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hoxxxoal.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fcvryshg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cunduvqg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfapygbc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bouljapz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mprefocr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ucxpinxc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gcgremie.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ylxqijvm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kqoimstg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dkkxqirt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2czlojcoo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sjoyrcsy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ptgxicbe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zdmrynia.html


<!-- 参考信息 -->