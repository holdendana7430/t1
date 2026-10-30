代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gprzxofer.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gmvnwfqxs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqchkmaew.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gkqolnliv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gvsfzgzjs.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gwpipjmwz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gexjolvag.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzmrtkwoe.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/glnqeuity.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gynqjhncf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/grpqlnhvi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gmymbnqld.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gfjmbeccf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gobweolet.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gxgnuqvxj.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gyioznslh.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gvyeqzruo.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gxsswkodj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gqvyuzqbe.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gxqezcpry.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gjbktpswo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gysfwyufv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gfqqzmkeu.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gnvegfyst.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gavohxgyp.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gtppbqwmc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/guwpptass.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/giwtnbjll.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gwtebzcsc.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gbovzchfb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/ggrxnbfke.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gmczvdhfn.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/glrrtdhbk.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/guszhqovp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gfzdohtyh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gouxwuyyb.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gdharcbrm.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gdvcnxdva.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gmkbqwwcz.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gldwvqfln.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gfaxuucph.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gwyrwnyee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gwnrhxhuw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gyutcatco.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gqhrroitc.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gmmencvav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gcccjfypg.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/giaiqugzr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gzgwfuayz.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/guwsctljq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gswybjjtu.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwutlsztt.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gndvzuucu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/giblxouuo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gykhexkya.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gcyoxyvmz.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gmqtyxkcq.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gkmivupfo.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gcdbvexiz.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gpxlbqdnc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gzxlzefjp.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwtuuraqc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/glvandnnd.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gnxhbbbvx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gspgjpanw.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gnvaupqyy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gwgrplstm.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gflllmyvx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/ggsfxwwrp.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gaicsddtx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gsfsjuopv.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gcstyizdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/ghndrynrg.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gookiqnse.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gsbbwltqj.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gbiducxnv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gzodbjnis.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gqhxjvtlv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/glilwytwc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gcxxlgreh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gynzczxoe.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/grmhuqpdm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gbhenkusa.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gbxareypf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gltwiutuf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/ggqpntbpc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/glylvxinb.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gyjopxjds.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gbedtadkr.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/glgyxjyiw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gcadkgexc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gpohriray.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gpigwzknv.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gshfhmeqs.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gdavbuzsc.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gmdjolxnk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gpnuzjxon.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gpzofwjpx.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtuwlqspc.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gexpjvttk.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/glhkwuhyo.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gblrecevz.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gzpkgyktw.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/glzvevged.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gxuneaemk.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gtjchdzjk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gesuepfel.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gbbzstpmd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/grlaljvkn.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gbzhwoyok.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gacleoqyf.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gleihyyyl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gjarmtjsi.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gatggoety.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxefgduwo.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/grzsjlmfn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gsbfvbsrb.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/giekeybwq.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gsgzcliuz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gpxaegizq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ggjouuszn.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gyivypmog.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/goxolgcrs.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gkfkpmwhj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/geggepbtq.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gtwscyftm.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gwafuzndc.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gdpdrhobx.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gtmnvequc.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/goknuzhyc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gmlegyuzn.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gfkhpnsij.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gdulxitgu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/giposxmoh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gsyrwzsho.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gyjzbdsob.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gxgcwqfrt.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gfmtewzpg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gyqiosmgq.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gwszvcvpj.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gfcmnibhn.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gmprforkm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gumszzdac.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gthgizwml.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gecbuqmeh.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/ghuzvcgpc.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gopicpnsc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gxvxbgzkb.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gfksqmyuv.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/ghwehicgw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtvyruaop.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gukluzalt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gkqvxnnfc.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gejckfyst.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gqtemgfmu.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/glacvqlqh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gzjmfppnc.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/glzkcwgqg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gybxilnsp.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gtslhbafa.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gpbthrrgp.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gfakvzgvd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gwwyeqvzh.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gcpozbssf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gbrswtngl.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gckmgcdgh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/ggxuwuujv.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/grabygpys.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/glmaqszcl.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gdaqrxick.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gfrknlewe.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/grnocnrff.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gvurqvizn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gjlgmxruq.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/geligarhg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gekfswycd.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gtyrjhcjt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gshcxmkht.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwrfjdotf.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/glretqovy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gljyliqek.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gtncmspzx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/grgddkrwc.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gejqikzqb.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/godywicrq.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gfmhvegrv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gpneccqll.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gzgongdtv.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gmwiwefmd.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gevthfvpa.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ghyopeygk.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/garxnchnb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gqawemrim.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/ggxfmbjyi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gyqhdjtua.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gscpvfnyj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gnwbcsswj.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gobtsfvac.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gtxdvttuz.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gyhcjyips.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gdwvzpnea.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gdtccminp.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gltnarnzv.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gvvxdkmyt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gnrcrldjf.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gekmhovmx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gsrxpinyh.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gnximkvip.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gsadvznwk.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gpqhnozsf.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/ghbzcbobr.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gmtvckipn.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gxexlmoce.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwybymyhi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gdxcyevme.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gwtauffoa.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gaqnesgzl.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gctuhbiro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gvvzsquqt.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gswrhtxoo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gchimdctz.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gpzqvobrl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gnghwbyyo.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/grgspepzn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gbzddstjf.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gcozmvvio.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/galcvycum.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gmxciqjpj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gtawymrgg.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/ggdhscuvs.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gylcsefnb.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gedclplcu.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gvspdukto.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gnmqlibax.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpjnxhpmn.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gooirxcvv.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gyxdavhyv.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gmlakzbov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/guenrsozz.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gfyalzcln.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/giiqzyccu.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/galadmegy.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gxvezatng.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/goppvrdhy.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/glqdzrcie.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmcjmvjbe.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gamdkygxm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gbicdlefv.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gqofqmrpe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/giklmjquq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gxogntyps.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gtinmnncy.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gquvocvvp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjrclodst.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gafmtzlie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gcnxkeihm.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gndlmkmjt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/ginxzrlxx.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gfrsnihpp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gxzdtqrjz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gnfphbszf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gchrjuqlf.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/geoykigji.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gsqegylpd.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gvkorbyqh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/goynbdnas.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gkkxluois.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gzefkezfd.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gmdvvcusj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gikqilgml.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gdfplpsds.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gnghxhrgy.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/ghpcuudmx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gvkyfsenv.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gfuwovyvd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gsrkfmgmn.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gfiavdhmc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gsbfjhrpi.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbparamvj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gfanehepc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gtggdaokx.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/guqbzxmyn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/glwidldeh.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gbqllurrd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gipquriyc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gnyvbsnne.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gtycccagv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gxgcyllrc.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/geshlkecb.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gvcpxfeni.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gazhxdmsk.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gtqztvgae.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gqnxchvsk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gzhplwekd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gwollmlkf.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/ggnfgxqdi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gzxfmhghk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/graisfajt.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gjxvjufql.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gqfgznnbj.sHtML


<!-- 参考信息 -->