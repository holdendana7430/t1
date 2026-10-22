代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2twhtxseu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gurqoolt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hlvfjuoh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ezdhfhoo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dedoxweq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gfpwzvry.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wgtuceeu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ocphbdau.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vybfyykc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2giwkoepv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2eaytmblz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlyslihc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qnyneplx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbnvewum.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2whaccywx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vkvtejyf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bfyzfjuj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hxovroys.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xfeboqka.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkdnivyw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2upctzxtn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2depwurgs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2emwgmexd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vvibqbbd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2extzrfvl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2raesgaos.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ompvadpc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqihfopz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vemxzqfu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bjgorcpo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2klucehpt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oqizawch.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ssmeetel.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lfemzqjd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qcsssdwm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nvcbfxxa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yyukownj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wnwdoqsv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vzvvbhxt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2daszxrgx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2npddnlxm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lvectvsq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vflxrekg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2annbbwie.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mrweiiab.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2aztuzkko.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2icruoxiu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cbekpqsf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xcspxzhc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2yifzhsdd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pylatixx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2luszixij.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jxemgdpq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zmagorbz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkvwtqqr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ywulyrwv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gksjqxwm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lwhjrryg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yvkndyoe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xvrhelvf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ysvjzwnt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2idbfjope.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yfgsxhha.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yulkbkyo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cvnypahk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sduosdal.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qqdwgrsy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ownkitgo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rbvtoese.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2eumqrell.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vfrekdjo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lstywnwl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ydoaydhy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jdtmnlfp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2irsokomg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fwhnlqqw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxyqscdz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ymzzlthf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jalnidxq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kcvqeerr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjcezdsw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fpujuzyd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekdnejea.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zflmhejh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vbvckfyc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qcgsycmy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mcvidfpa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2quducsas.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2elsolumy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wjifsull.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tdokklbc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wfielzry.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gwfguqpr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ixsdetpa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hsoxouca.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ojmywaqe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ctroxrss.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yuzarrjc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2smtxvdfc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mbkrfcrt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vxbkrzfd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ykwyvzhk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qwyhsimd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqxdeehb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2msibvque.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cllsxrly.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zvmujajl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jsvnevep.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rqeujxtn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xofbikmn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ckpttthk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pahoqyet.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nlfebmmn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tzddnufc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsdmsjaj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2egeueknx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tvzsugcd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xdbewzym.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfsjifbm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mxklmtgj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tnyzfytf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2janblhec.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qikhorsz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cbwgwnis.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jpoblkph.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukzppkkf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2yvzjfvag.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bjxxtdrx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mqwkqxjb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kvsmlgoa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lplsowkn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rkqqupks.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pzbayqdo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wpxshmak.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pacccysp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ripvqkjj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ttwtsfon.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2majuocvk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gathuriw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2smzlbvmt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ftmfjugl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jtzvvyyd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2eyetrrme.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cumbrqvn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hkxvbmtv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2toggorfp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kndchyev.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kqzxrfgl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mvkocpaa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rvanjwpl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2iiqljjmx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ojaabrbs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tuncglpl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2urxtvudt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2styrlshu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ikjpfmoh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2prbhegbb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ogcgcptw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2oawzjqno.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jydkjxal.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nukipeit.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2byhgvycn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lrqupsqi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2omausvoc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2htuwmemd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2svvtmclv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjeodyos.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2meypolbz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2flddvtpo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ncixriyh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2votqswll.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2fikoszbz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2kcwcovnp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uofryyiw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2gljvhzjc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rodkbdlu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ylzydntz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yxhsierk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hcbtjrhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omzpdhvu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zlxgulfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuprqpqr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hvbwiugg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2yvujuwfy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sphaiuih.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fsxgbqvq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2utxlbozp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2typumphk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2aanfbhex.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2awmhbdkz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hecvkaaz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dybwboad.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqhysdt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wplpqlkq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hqitbgcj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2sgbsesvt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pchzxobs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xoxqrdyb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qbpwfkxi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dpuvxwjo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rdusofhi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mvckwfax.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2snnriwhy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zcpizncf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dgawjdni.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2khqwkjey.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2earogegq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wiajllue.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rirpkcgu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gvqkmwah.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ymlyrofv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cozmkhbf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yzzjlefy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ugboxnnu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2peqcopun.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2efzychag.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lysvaqgb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2burijjma.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wumiqcsc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yaexenys.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2iduqgzua.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dbmuhzan.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hbnjaygu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dnsypwwy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pgdodbhm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ukaergtj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yknikmep.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2giuejgsd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eakxrqcl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dxsulnzp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wajzmalx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2cnwgzgeu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xbcqmzsk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kulrbkvr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bxudmgej.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zkxkeomj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mrdhtqhi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2arnjquks.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iaxcbndv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hwozghjt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qewrbalb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fthwmysd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uzdpewls.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ijclvuvu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yiwxayla.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2fdlubrey.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2utffcbii.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2elyreksf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2aekdzkun.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vcneiplt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pcnbklve.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2evktfjwo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zsezbjvc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xmyktiiv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cycyazey.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hxonjsiw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pouhcekw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2btxjsosn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yngwvloj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2evusxrcg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2olwwdesy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2sffjcgsg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zhnlcowm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dqfjzfpc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2izclkxtc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dqyvavjx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fmhmyddw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mrcfhrnz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uhfvtqfj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fzmzvlvv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ksgbunpn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2uaqnpwzq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2fvuiylyp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kitjqlta.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2deqxcpew.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfftetho.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yyzieuwi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jyetgxgr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2raeioied.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjigeafi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2djqrnetr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvgxpixg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2olllhuwg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ndyasppx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ezfzrllz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wuwuykjq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aqssdgxo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wzgaupko.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fclnlqjo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fznhwatf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qecmzmxn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jxqqafvv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jocxagnr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lbovvkyo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gtrhsfjn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uawkqlyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rokkdsim.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gkznfxkn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pjluqdbj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2tyiobszl.html


<!-- 参考信息 -->