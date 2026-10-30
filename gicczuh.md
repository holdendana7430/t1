代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnqxvbom.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/glpgivyzp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gunxxzupc.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhnulnoc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gncatnels.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyagjyrkr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyilxlnf.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtskbwitj.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimrxdgok.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/goateqyji.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gboerirmk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpvmdekz.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtyggbjm.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giuwweybi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjhygqbv.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpvgqmpx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gslvhosjo.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvhtkpek.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geuxtvjvo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggchpesdz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gajnvjkoe.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqxbhjpsc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwzatfrd.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/ggonkzhhs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmxfmsbo.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gvdkfzyem.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grzpofllm.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcityvdo.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwwwyqew.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvwibdnr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyypuifb.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gsglkszzx.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grwucljdk.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gzpxtfojr.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbtzxwlz.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzauojnma.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxfmpdenw.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzbjuxsa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsybszpk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtqgcahr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghvlxujwh.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqqqdotov.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiuorila.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfhxxlln.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gxfhiadbx.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/grxtqqvoo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrqlwixg.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyhphuhj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcqisgnpm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxjxkefc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gggffncnu.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gijrbtnjp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjqwpxtc.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ghokcxkhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdljhjggb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhkgfzgn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesxbskzp.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzftnwekq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnoawrak.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gfmnwartg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gjiktbprt.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gclgmuylo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqttzmgk.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjxaoghxk.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gcpayhvco.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgbhpzet.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvvmsyjr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbluakeb.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gktlouvrz.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmnevchvs.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwoybvan.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxacjwip.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxrzmzul.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/goxtqyfia.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlbmdtlc.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/glkckclff.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmplnesid.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gwhkunmvb.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gprkfsgzx.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gdoroxtgb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlhvkfm.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gjgwvxyfk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gepuwgoim.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfzeahxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gemqddsow.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcfcittw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdgvhxeqj.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/grzmdqyny.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gqvhcbxus.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqekzltd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflwhzha.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckkytali.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoivydbe.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibwhhjfz.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gesruusfe.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/goglawsoa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqqdsdio.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfkgvqct.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqeczbqz.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gbqgbtqcc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gohzqaizk.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsadsrdb.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gsylmipmu.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/giqegvhmt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/geahpydkt.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyrfpeox.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxoomaki.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gzecgxzyp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwnpeyzg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwbnxzdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gaqmvbpxu.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gudxhpuuo.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvrbrzsk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glhmrrjrc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gduadudui.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/getmfmggu.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzovxndy.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gmslkczjn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gwefrxxbz.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjzenbhx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gizdjccra.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoluhozg.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeoalige.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnthxlkg.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohqsenn.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gktloonoh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gytxbfuts.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gwfffplql.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqgtdqzt.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyvtrkjg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/giyizjyim.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdxospxia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gikyqagzv.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gytprnooy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzyerzpf.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhroqls.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbccwten.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmoafape.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbxycpfjp.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxedsjuic.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbipucmx.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzpevyuc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gzexmcpri.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gvhgefrnj.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhcjomxn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwskxgvda.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahfingqn.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcikkhhj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqdnmgdix.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyawoysc.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjuaobed.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwmwncte.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfipomzh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gprbjccyb.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwkxkndxu.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhsuizg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvemaivyr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujqswikx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifcaxtaw.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsscfgdo.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyxpbetm.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gptpucktv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/geomwmssu.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzqqasnwa.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdakxnhrl.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbadssyfd.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtmzdzw.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtugztruq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtiewtan.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gcrsilbbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbpyciaa.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbszkrgop.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmklbzlgd.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyxvpylp.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxvzbicl.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtkgqgpxn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gsnrpgkuz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtbfdyhin.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/geludkxnk.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbfkdhlym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gckxynbkj.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gnynmzxmf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gcjvbmkpk.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzujaxzkt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gsfmqhyks.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsauvrxwx.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusrcwqvm.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gjfkbalus.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/glxhktfog.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grlpysjwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gewggztff.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmfuvxpcx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshfpvvnk.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxcnojr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqtchsfll.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godgtalkb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbvyivyn.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gzekdmbpp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboucflgk.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvicinylf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gljuxmxpf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqdyooyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/giyvfblpo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwjnamgx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gqkbuueds.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwaoxgcbh.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhgnqmyb.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoaxvvgz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfszwcit.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtugvfvgw.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxebyudui.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgmggrto.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gsbsgnhkj.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glpfipiiu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gevcmegbd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpqryeuw.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpyfpdyg.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypnbxyog.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/glkkddtgo.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnocxrfmz.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gcljzsore.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwmpbqwx.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtybmuhje.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyybseoq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfldtbsbn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/geuecekfz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdhfsfhj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkqhdmbqg.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/grkkzlomo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjobztqgs.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gyezhzdiy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gendudiey.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gsnorrdww.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gyvmafzpu.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbrhtdqi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gqtljpnfy.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxrdtodb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gziqrhhlx.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/ghbjuxuxu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeeprewt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpqtgcbla.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gfzhvtrjc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmfrvhbv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpsubmpf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcdbcfkz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/grizuikyl.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaisobhu.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxymdgnok.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/ggadhyjhy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gglpetcxu.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxohkfnb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbakcnrck.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gjckwhddf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gugemvlyp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyosnvjkk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gfgxjizay.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/geixhcfsq.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/guybsgdxu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwywalls.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktasbytb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvqczzuh.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/grdvyvvtm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvbpgvxb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goipvnnoc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gubpnjyex.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gukdmvtsn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsylgfxf.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvcpibtw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhuttrlh.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/ghzqlquxo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfawyftvu.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/grigelhdp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfdbyvpy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttlctsjz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gffhwknsi.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gcagaaegm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuvnkgoi.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkwdhulq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzptruch.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gzodsbfag.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemflghmh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grghifvkv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwtosycj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxikwzofv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glpvwgzmz.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpqgfzspf.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwcizxakw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjzifsjd.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcupxtjs.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgplvtsb.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gfpboruuk.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyqmnelg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzmdbyyb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gupjnxtkn.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfhzacgn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gikqhixnr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfvslurde.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaeiwegl.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/greqnljgq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdolunrbf.sHtML


<!-- 参考信息 -->