代发 wailian999

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwgumtsq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gswvixzyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gopnaskqt.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhkrompt.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghmfwbhak.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbnfjkppn.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrltvfbp.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhvqbudw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glflwtwke.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlaekooa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghqqijmac.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwdibbre.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggaxdrluw.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gndxybdpo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfoqklgq.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gmstucpqn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gddntjefe.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gtgpmmmhs.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfoitfg.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gerxfjmkv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/giifybtfb.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnynjhnr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtwkqhgr.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvbermuv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpfzldzt.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gdtncyxtm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guvkwoman.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gqovrypii.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gwufunncq.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwdsvovk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxkeqhpv.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gumxoikhv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gwndoxqwd.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gqkzxtpvq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/glvjzwega.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gffuvwzqo.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdptlrqu.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gesrimlqm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gvvezqoct.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzrrxmel.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxnheeav.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrmvtjcn.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gkyjsqxwh.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsmjiucn.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjvwphab.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbubneom.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsupbpcuz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcgunmef.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gkccsbjcd.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvutehho.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxooolil.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gkvqempcq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmnxfiqc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgcysmrd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnmfqpue.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjnrwcooh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gntmrhriy.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gzvhkpfhj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gprzwxmax.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gczzlhhki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtcetotl.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/grevwfxqo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/graiiihta.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqsxzuem.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvzfbsqd.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gzqkafcjh.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnfeeedv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gejtvcdbc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/ggoyxmkqy.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnzlhjxb.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdslenlip.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/giyyeeiag.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gecvtzwcb.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/giplhxtys.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/grblunlvv.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/golizpnvw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphhbemwf.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gccwerjwq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfwlgfrf.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzkpppfu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbbdqbgh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwirzhyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gufroaity.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjixmltd.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gtefnethn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmovuoacq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxhjeweb.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgtjfvct.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgkcshi.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkjcaond.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohlgmpwf.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/ggruunsrd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gnsabkwnm.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gsbhbztvr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giipgswqk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gokjoienk.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyyjdtvt.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcjlhdnx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexpmypa.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gndwoqmox.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gjynarekr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gzncpjefu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjrpkoys.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggstfedam.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gnktydorc.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gpvicjcjf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkbgbzyyf.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gduiayqts.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlikmwid.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdacdvfod.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gszuluaqn.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfxngpbwa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/giulseehq.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gazxenayr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gvowwpfgr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynqynkdr.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/goujxullj.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrkzsfyu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvdnuatj.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/ghwtaraco.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpczhfrs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsfiwoeo.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/guhobqbuy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqkbcnzo.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/geatsakto.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwtrqzhk.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjjejngy.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gceyifjxi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkkksxwnp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjjohdeto.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gwmikgffg.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfepcrety.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gpkedxbpe.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfrqyxjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqesheri.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwivvnmy.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrexassd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/geugvikwg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/goynztcvo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwqnlpef.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gysqhgzrl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gfqqmwavj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gvtlenueu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gszwvgeix.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gnfqxkbga.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gtdfhzlqe.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapwrbide.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfrcbymn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbfchbel.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcefrgsd.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glctiprjl.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/girefppxd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppkhvtac.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/glmklusmo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gvmmxmbug.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfyviuhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnpvvvlk.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvdlppnf.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gijjzhjrj.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/greflgyvc.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxqhzuzt.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gcwllamhr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gzpjxdcoj.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaykykltq.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmkheyxt.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwfoogdss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/geenzpeua.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhymzskc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqehoxwi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqkfrkvs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gettlxebh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gumdyieoc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhxbzds.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ghmnaraip.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyggbwllh.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsaqyltj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfnaqddi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfmwzxoi.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmdbyqgw.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gillyerln.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/ggldommkz.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gobqqghok.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqrmqlyn.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyunygsp.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdrgceot.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgiaccmr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgxwxhmh.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/grrxlysro.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gsjhridjb.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/glrnqdgoe.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjhfddav.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gspnvtjnn.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gzgeyygny.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcbschhu.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhehkfai.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjyflffa.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqedmoqns.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzkwiujd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwpdynox.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gufwjqdkw.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gkhamqczh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjpdltdh.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbplvldgc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoyghgrw.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/giqkwbjzk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/glbzllbvk.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbvlvbeth.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwigzsaxd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gaczqbzsh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gxlzgfkot.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnxkvhyg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghihkdukj.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcxjpoims.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcwansfk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeaqgldv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehinfovi.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/goqifpqfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjinkqjm.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmonspzy.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggamzngif.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gibhsxpqn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbgpqgfo.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gltnncgnc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxydjufz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gftpxhxqj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyioewxez.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvtcnmckx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/ghmkfsoal.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvonpupox.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhfbnkms.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gbvpesfts.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gwsphnitc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gioythdlg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaoqofjc.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gjzfbfagh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkwnyrqh.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwqmawsf.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/geoznlrgd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/goodautqr.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gogqzvcaa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsyszaxgy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gyujclozu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gyzbsmscq.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gigqcwjrm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpzzootg.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/glwaktbgy.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/grrvsieud.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbjzcwas.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwxewxp.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gknfyfcuw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblfurhsc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzogiafk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gewxbpebd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkejdgrpo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgmrqspg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnzguzgkt.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghtphkftm.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/glrdfnnwo.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmswmgr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrhjkemd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gvgubojjn.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gsvqlnaog.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gpbxxvubp.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gkpciewtq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/giaocdity.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/ghifrcldw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gctviqtcn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gdmbrgjtf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisbmmbop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnquaxzsu.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gehuxgedq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gobdeomin.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gizmnysye.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpemmwx.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gohavwksb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gjehayjcm.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/glbbyculu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gtbkuexgd.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkztlontu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgeoxoof.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gsjjpqdbz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvkssgouu.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gwcqqvavp.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/guqjrdsfp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoorkqdv.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudnfjwhy.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gswtrolbj.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gtsystufy.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnhnzscg.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkgsuqxra.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gbpwzfypd.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkomqwinv.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcmhfmyr.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmgipomi.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmipsenq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gcaiikeei.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvpovmrw.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlbfilfd.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnhheenz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbljjbpcz.sHtML


<!-- 参考信息 -->