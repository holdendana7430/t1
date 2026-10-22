代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xdnzzmpa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prgycvfn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gemvnmxi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjedkxgg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pviledaf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mipyyxdq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2txnsesnp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wgkwpgzh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2oifdifvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ffeoaqzm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2mohycqwx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2borrvciz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tpxelorq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lkgivxbe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcijnjux.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kjsemsgp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yjwdcnoe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2aupzuyec.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ffgqeumr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eiwmulga.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qixjgjdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfkumqcc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tghxgthj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mkiqidrm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2autivbxh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tepzcfia.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yugmmcuc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ysauewal.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vhhzplde.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sgpypxmp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nmnijgln.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vsbojmnw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2turhsgrx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ihetqoet.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ptexaske.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zdjwplpt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wswkcjxt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2chidvakg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qiwliemc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jtmnbiyc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jvpodkqv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gigwumrs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2oefzcgcl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pyljdjjp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2fqcwtyfn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sukrmxxw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xkuovbcy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vgjfkiow.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gmyjnoce.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2atdoqqcp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kbaltqbg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ytokqcat.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2npwgpglq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yhklebee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ykysomji.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nenublcs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2czjrifds.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pecgahtg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pwkoruxa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bxtzmdok.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2duvwtdtg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ygfwvbrq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iifxnmvy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jmuomuei.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jttvtvot.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fqowpxrg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlifhmpa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vtbenilc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddbjgktk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mxxcicjk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fmejyutr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xeclmfqr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ssmbzwov.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rfqvhdym.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2skemgbwn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fbwvoduw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pznyxjjx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zodjbqbh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mfstodrc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dqnsrvws.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2suuixbqk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2phobegwr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nuhslalt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yfcrabyy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zcvseadg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ezqtgkgv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gqbxkrvk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uncvokbx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwixoumf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ddruxuwt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2puvhdsel.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mvrhxaqg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ufpjfydr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ccehsbmf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bdwdwibw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mmbhwrew.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2wuvsldyu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xnnmaoal.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ofbdysjc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2twaluxfu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iytnaqfc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kgauhnxu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wvmkcplj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zthxizhu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hssbeahr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ckwadljb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2czfvbfch.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vdbagshd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jmibxwnp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lhblpzvo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2juhxwgvp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2swimlitj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2eaixufpn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hsldickr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bkirqbiv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uivzasti.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2suxknkuu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jekmsuyi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2eupihmul.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cutxmlbo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tffdybbl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uqgcffip.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hxdofllk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2eknivlea.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lxxjvaqu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zaddcaqr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfgdqvfu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fpkcruke.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fugyacto.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2inctdxjg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsvdgbwy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2elrfhfgi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ulkhhkqs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ovicwtyo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cqblocdo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zyczcubd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vqjknxov.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mtvbxylu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2arxbsaao.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ptbofauj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ximihhds.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dansozmw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2olqwepjw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fgtyfbfg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jwhgrrhx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ctmyzezo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ijvfaflf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sqpieuck.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xhkdnvgq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozaaysaa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2quwdnviq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2aejcuact.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2suhvczfd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2okkihaaw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qkzsniql.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lxhkltuh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2sepufofz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2prkpsrit.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dcenvues.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mizzrgkd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hbubhjco.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xrpkzlhz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kjioytsa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uexomqan.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vqgqkvgt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lsepgubb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wgsobcop.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uynzxycd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cbxoifyy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ytbdxaja.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2netnczrg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2clmnsell.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mmulduoc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bbynwxvq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvixhonn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lkzohfqs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ubwqmcmo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jqyvzzgk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nblpnodx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2iltvforc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2eaeuwfdl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dmsfncxk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jpogcgmn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lzavmdbs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbuunsbj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2txatkujz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nojwixul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpjunnyo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2yrlpswej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usmofjac.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebbavfxw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2iefdbhfl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwsfpzxs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kxkahheh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2edvbuuze.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2soubvjln.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2aqdyqwxf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2piylvzrv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xjianmsr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2knbbjvil.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2cyjjvtln.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jjiatltd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jpwncwih.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tunjjmwo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bakghdnn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hvbuujof.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qftsucyt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cvecldvk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2agovdhgi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cskrwddn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ferhvixr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fonkkimi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2smvqvvdi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dmgjkpvv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rsutecnw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wllofgol.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vffxbaao.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dysztvgy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2sheajhkr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jqbztvqs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gnumhlzm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lxbrjgcu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ddpzlqus.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bmoxkycw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2peghimbr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rnbgofwr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yfmwspjc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2huerrccp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wvsatwdu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fjrdkuer.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dyuhqwyt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2khxespss.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dfacfqsl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2segrofsu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xwdlhnax.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jozbtnts.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cqpapnpq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ijehndyh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2plxrqjzs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qiykdkvv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mzwlhelh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2arqegbrk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2omttaocz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2igxqecnf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zivuaovt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2imglrsox.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2swlqpzeh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rgpedbos.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xjbyyqut.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2aeobdeda.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nflonwor.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cbxrfhor.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rgavgmei.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bmgdtnpf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cdblhnnp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jjzbvqlr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hhruoczw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lbadyakf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewxuvbcn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rxtmkfoq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vzfmhsuz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ixpxqzht.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dmgoqava.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2slmqhqfd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bragahbg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yjfwnkml.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ooyxoxty.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jprfiuvk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yptmmmka.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kldupoce.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ozqcvpgs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rdpnmfor.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ykpixvmv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wxvwqnhv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bhhophph.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xdiwlcdb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkmlewit.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dtyixxzc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mpyqfcet.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sfmnnwzd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sqdqrtul.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2syomrujh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fnryvzzs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbhizdbc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2awrtnaog.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pgbwkojb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mnwslkba.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxkljblw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cwirvhrj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wkrqofhp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jqjsyxue.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2juheswvb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qxymnoax.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfwfrdvq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hihpapif.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xvcnmjmj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2umkzpxqm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rnrqlxdv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mlkaxblu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gfcmfgoe.html


<!-- 参考信息 -->