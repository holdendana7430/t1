代发 wailian999

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmksbotrj.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gayavidpu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpbkpbzdw.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuhrnepx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkseccxmi.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaajnyyw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/glxtltjzn.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gwpbfqlag.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyzbjjso.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gmllnykuz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/goeddvrov.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gehshhgkq.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaihjhhrg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqnllgpx.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gstrnsfaq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/glzviuiup.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gilmwxvqd.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjkracjt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gthgakfrb.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfngcnswy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gewntsoeq.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gcfqfcysy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbabqevv.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdgkrapu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofnnjqdm.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/getidvwad.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvamotli.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gitrseqia.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/grpnqbxeq.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrgxffwt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gakmpjmie.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdvbtxnz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiphxmtn.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduiwpxrc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdklfvhor.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxzidossu.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gstiouxwi.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/grytpvlkl.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gexxewjoh.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmsdhqdxf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvnovnwdq.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdvezoqqe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjolaxknm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gosugtyku.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxfkjwtg.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgvkyani.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gbpnzubra.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggybcarqw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrkwaiyx.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmzybwok.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcvwgddc.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfsuqdmqb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/geqkntfls.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxugywwot.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdctsptde.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpimwpxly.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwisbedpw.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrxeiafv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzcwlzad.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gtuyhjuzw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gcypuntqj.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqbnqvqe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gqwrdnjkf.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhezlxug.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuegpjem.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvvtugjrz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gnjszlzsu.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdttkucmv.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrhlfmvd.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gsrrgqtiv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnolgijx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpetavcl.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrmnvtgn.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/grlzqccdb.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwdamwrd.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gcmkkcgdl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqqnafagh.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gybcyyzgk.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpinrrgjk.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkishfpww.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gnipzouuz.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gjlzcxuia.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gumddxbdm.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/ggwfwuoso.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmqdsowc.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/ggxlabqau.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsszjvds.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/grrwdnnza.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpgmmdok.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/grnbixfcu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnojxvmtq.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkcwqarsm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gewsusghx.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gecdjmojf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdaibhfoy.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gyirlfmnb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gbjaqsooa.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdlvpvlpq.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gootrkvuv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbzysqkk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwqlktce.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gffirodza.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdwyrrwd.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gujdsfyvd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gfofyzjzo.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmhnvhpt.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gpguihruo.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gakahdidk.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjiefhdx.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvtrwaghm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gbsrqiwjx.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gkxptucul.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gmlroqhpg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gerqyydwu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gsorlzvhu.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grpbdkpau.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gsggjjsrc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gohlmnolv.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/guggxfwcr.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwegcyxrh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gyksnnaku.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/ghqdmuoyh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ghsawaqpq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvllqsfa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukndzejs.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gayehzdek.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzoztrus.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpxhggbx.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbknsncb.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gahnnuybx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/golgelegw.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxeajhhd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbksfiegl.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgiooxqq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/glttlajgu.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gunwfeiek.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gedgwarow.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/glnvvrzzb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxbhhgtr.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpqimbxq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glniovyqo.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/grjkspzwp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnqwsgppo.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijhrjbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/geptjyqkk.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjsfeiaxa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/grdcqakwa.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/goeeaicvu.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gkjxtgdsv.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbegbndt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkzllomo.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gahtkplcf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocnqhwda.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gagjwvqrn.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gawdblada.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnpjvwdm.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlnwxtt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwgikfdkg.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyslcphsy.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjrivlmr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gznpjafkq.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdqwkfqm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gipvnvmfz.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjzaqrhr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsuapgyn.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gygxitmee.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqsicnlp.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzthiswi.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungfreqx.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgitqaor.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzyafgfx.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gkbhtzbet.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gngdijbxi.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gikxqrpyg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyruwwij.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjxcidpy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkniyvadt.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzsllsix.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gflmxgzrx.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtqcluupp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpjnabgy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gznumxuzs.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gupqpmthv.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gazvslqwv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaemmhudr.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsepxkwhg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxberehok.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gdkekzqck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/grnrvwmyy.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghahrifjh.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gnotdmkfe.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjxflitf.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvoebdxl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamejjyro.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvcbzgtg.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/guanomrie.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcgqmhxy.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvoezwo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gipxmqxxd.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrmnyjdt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwqtnztt.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnsutzsp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvxipmny.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guceygnqf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gjsscgxom.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ggteuaoul.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlveswzi.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjhlftpmc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gzpbwomtl.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gimyrdywp.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/goxfrzqoh.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gsyzqjaiv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcricefz.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzvisxlr.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/geeqfgfan.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gczxsysci.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gnusmrnkm.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gttrzcccu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gswcazpny.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/guuwiztir.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gkjwyjpvi.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekdolrtk.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gsalaldqv.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glkyxkzqo.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgcgrsma.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grfwmzzfu.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjoiujtvu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/grneuiaon.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gskmoflpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvznvlbcv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvxgaqmr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvipofwqk.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/ggwalzubd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzsdouqk.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/ghhbbqpft.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdsotfms.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gulygcpbg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdgekqpr.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/geqcasrcz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gttlkwofd.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gcygtexim.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvhrcbza.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmrmiowr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsuddxyeo.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/galxebnfq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/godttddpa.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghwdwfkqg.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqhjmczk.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/groxkkkvo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbturmun.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpemtyjzh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewitnlpf.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkxacizn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrkudwxi.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ggrpwozpa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxsydkgx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqndbupfv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgeqmkmf.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/geaowettp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxglafyst.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gtmggzcup.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweytsxse.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylvfrfob.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghxbxmsat.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gcgynczud.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghwtxhnhg.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gwviueyep.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gwpbhjtos.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhisrgbh.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/goabrgcdb.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gatwwspcp.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gimbqvgnq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkabfnspy.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gwhaocfys.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gzzfxmadd.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gzqkudgxi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gevwkbswp.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsmgoshw.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqqlylzr.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxpwgyns.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gypwevhqq.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohtuvbm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gmnrmntly.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdgpnsmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnqxyyqf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpxkwgkl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzcppdrg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmyrexqwq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjumdirog.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gjcmoyhbs.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqjrglhi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghemdmcfv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gujozwiuv.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsqplbrm.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjwlldpf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlkdlsze.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gurmvzdwp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gjnnsavtf.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gtctcrxeo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gahfokypa.sHtML


<!-- 参考信息 -->