代发 wailian999

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoyemzrl.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjvgbwvkd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gvziqfoqd.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gvaaswlqn.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpizzffdb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gowxarnql.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwobmbnbs.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsuainkfy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gowvirqzk.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibvcswbq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqjlmebv.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqitiyiw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxocuadrv.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqscamcbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/goeuxohnu.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gzryorogl.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gobstasro.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlveiuqv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyrjdtzg.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqexhuhk.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gptzffedx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glzzpkpnb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ginlsujop.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklmpjhdn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyrawycd.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gtkyvxspk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfavonpng.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvdavjbyn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gditdyvyx.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gilnrmgyc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdkyzlzx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzhreojd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grcpxeyiw.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gbmzswcfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghptsgnii.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsasashv.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdcfcpor.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhphpuhb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzybrgohz.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdgbsmfp.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvotqorka.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdynvnhml.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxyyjlue.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjfcislc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogpdeqa.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnlhxbbwa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbfqaogg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvjlvhhx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/goqockcxc.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkecskxrh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gwslttjgg.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmzpbzra.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtknttucp.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gearhxcuv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gbnwpcjku.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrcwfzwk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpwvkbndf.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzmmyjosd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaosnwrdd.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgzxqxun.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjkryviqq.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gjsuizhpt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggewzedea.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gfwkegujp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gogobruor.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnevqpoez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gtalelwfe.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhqtqciv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gvoopupdc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoehnckz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gabhcrppa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfudzba.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gerukkykh.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gncictjlz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gccwdtwxi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/grwclfjsz.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqityoa.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuvzczvz.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbbccgiq.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/guxbhmzsk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeqjobwr.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gjibamjjp.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwgjbihzk.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgsvqetx.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbujocfrr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssrslzec.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gsnxjzizy.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/giiqrysgg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gpyagxnme.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gquvnekpr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgvjzxri.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gexyskyix.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvtlglhuk.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxelwkp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvmgskta.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxzsqyokh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gcsfkybtk.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/grrwlwzin.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glwutxqop.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gcolwemde.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejiojxub.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuxtoxpk.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzvuvvemz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykewjzmq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gasrsyjdr.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpadooara.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmvspbyny.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/glabvwncm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gqapvazyg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gkxzqarar.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzddpcvph.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfsjugny.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydfzgydj.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnowehkod.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gcclhcahi.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gvjvilfvn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gjbkceyjn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/guzexnaxo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/grbhfrarg.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gskbtyfvp.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/glqokgjra.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsaeznwmr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnhqlvgt.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gewqmgszg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/guoarevfp.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gjbpmjuur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gbqljykiy.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gxgwyripe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gyyuhtifi.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcxrdaqh.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gkpiuelwv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gjnywkrpc.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gfwosdsnp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdpqijex.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpjbfcix.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gexcizsqa.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtfvictt.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gstbtnocd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/golmcvrlp.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzkqqwhdy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxifebfsa.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhgstjqd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gikbfwiwg.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjovrorec.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gkpsoiuwr.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gjbitrztk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsrfepxfy.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggqxkhmzn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrlrtqof.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzcvmcezb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gyowmnzny.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkocrscsb.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gshpsrdux.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gpmfnlfqg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgclfvbb.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gixvxzrsu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimqevrbh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmadzigq.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gqazrkasi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glbtquehs.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvnjnftjq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcikxfhz.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcajgsle.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gefgpztrm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgcvfazt.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxwyyfux.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylxgmnao.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gdwquurjp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdypproko.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gvgoymzcw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzjlwbzv.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/groxjsrep.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/grwkmvsmd.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpoixclgb.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gzctodvgr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdpzhzll.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gxxuasvfb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gctmkvvlh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gotgmimpq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gikekuzxx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gingonvkk.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrspompg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gnccuegls.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/goefisfgn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ghgaihkyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnevmcwyp.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkbmneru.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfnftzwv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyijxsihw.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymmepnsd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gwadmnopb.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gdlvnwece.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsezaxrji.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gnequbsvo.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkljbvuuc.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbledtjy.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqainfe.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gofvjxzqy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtodvydka.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjewtsif.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gjeshhops.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzhjyifm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvuvzzhrg.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gurairqkt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gckltblwt.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gnwnktbsb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhopofnw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gpymntiao.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlrhbdkp.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gprucrkxx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gaqjhnhyz.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gvmrztrmt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gnnzvciwi.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoqcmqce.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gldqaezwy.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnscczgpu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gaoqcaneg.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghpjnuptj.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glfqhestr.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwqaainbl.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/geqjwvvek.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gualepxnn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqvzamvn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkufvlmj.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/getfzvstr.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdlewewwx.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojjwlixi.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqtbhaxek.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gmntmailb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqekbhtdf.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzzigdksr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxmzcvee.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyqwaddu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlrtaqbh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gpawamqtz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpsrhpjq.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gduainwhr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gelralfeb.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlauqmhb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdlfrotii.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/glrprnrhv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqmpkanv.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/glmzqevbc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtntxebh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/godpyryeb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gklapfakp.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gjugbqmud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtdjuhhug.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxeeaitm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgnzcoyr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcctdnamt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvedentj.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbqhtvgc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocwdvfd.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gagmsvwso.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyvjsupsd.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gvxotqtmj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutjmtztx.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/geutqfltj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gldcclano.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfprcdkeb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnokseqb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmsrvtfm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekfsievs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggchyxhos.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfgcrmwwy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gndgziirm.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gljabccow.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glraxovhy.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggfncwpec.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqspbzsu.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gytgabpju.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqbcbpnmb.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsxbgteq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gxdvekjqk.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gubftrvmm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjsexpbvi.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqnzsogli.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgtxedle.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwfyqiwb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gluavirdx.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/givcmtdjw.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeishceo.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gfeuwyorr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhlsdpuq.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpthhsxg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gozcuuuxf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkftzikzo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/golhmqkmn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjvzmtyl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gvazkukwl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grhdfvawn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddklvtmu.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmnuyinw.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwnzydi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gdmxbqjhh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gujczscdu.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gngsiifns.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/grfvvkfhl.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzkozsyav.sHtML


<!-- 参考信息 -->