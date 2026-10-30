代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiyejsms.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjdzxhiqc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghclcioaw.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmejyeadn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkrurhuht.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gegdwfnjo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gonbipbbg.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnhcvnnff.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhgcwphf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gldnpkbkk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaxcsgfj.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieiemmsf.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahqbvjzk.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gywnupmto.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjauwjxx.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyawuvsuq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtzzovkk.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guseqqtmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gblpdvbgc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzkjqmdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcjjpqda.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpibconwe.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gqhpxbuti.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/ghikpaafy.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gotengufe.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/grfzduzwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrjwunfi.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxndmwo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/goornmneg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhntoeok.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gnjquoldw.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gntcmromj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqmkwlfnd.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltxzxosv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfirompc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gwyfukjfk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfowqart.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejfkssfy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gslhyfbuh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquuxrpxw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gurydxgdj.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbgltvmj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoeywiuv.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/grmohfdlv.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gikfthknk.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/goiquxvor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gtapemush.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gcljyifjt.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/goqctodpr.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqozzrsod.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzgcvgoa.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gyqluujeh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gfsvgytez.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedhqssqn.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvoxqdau.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxczbjo.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gomqchsuq.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gkspykxbx.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gwsxslqst.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/glaeipttn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gwildjqtq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gaythhggp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gukkveozu.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnblszqgb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grbylltjp.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpohgbsxu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geuvdyhth.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvkxifayr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxysekwc.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gijfpbbdm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gctxzslxw.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gosugzafk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjshgrms.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbooxiaq.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givzwqeaa.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvwqqzsjg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/geygmslhs.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwolrzcjd.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsobgggpu.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gycxsoijv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gcmmiguux.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gclduzuko.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gxtbdglij.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhygyrkz.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjxlftto.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxozassru.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gublnzalp.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwgxwuze.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/glwhodveb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gouorisjr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gsekxdvzr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjcbfjpx.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gfjsosdmr.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxjzsuwin.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikifgerg.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/geinxwwth.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gcnkpkcgi.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gtjggglby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gordyeutf.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/giiilxiqy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gyljrjozh.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gopyqmcxb.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gsokdztmd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gnyxprpbv.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhahvmor.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjrfumvm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmokbnto.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoukhgjk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpfkzkdn.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gjelzrjzh.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gbpxsbdvy.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbvicuzn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/guiilsbqj.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gicaspxea.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvxlapztm.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gponewhsk.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ghaluzyjh.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwagqpqp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsnbnhxy.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnpjlqur.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/ggcltphlt.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gewitzgyw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqctobgu.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeesmqkx.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmtxwjhr.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/glakkbakw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gampfrgqv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/ghshpcuqb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpjzcddwi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gmaxkmzuw.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrvjkfln.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvslssmw.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gvwvrkcjt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxbyefbb.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnchkjgmf.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/ginsvsvju.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/genufioyh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauezzsca.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/glvffhhgo.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaeekuoa.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goedyqzdj.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/grcsfkhvu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gubwnpsbu.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gteqerypg.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gclghtjtw.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgegrwtg.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gbujywjpg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvggyqan.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzksowdkr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/grxujymyk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhiadhaw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gyvscirmu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gatltsreg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfkvdkwj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgiggymh.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvdndytia.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/glxvymdxp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gbkgonhob.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gwyxoastb.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdopruoct.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ggfbsgalc.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzncucfua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/giwlwohjs.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtwmhrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gucgqdvee.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvamwxuol.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gnnxgmllk.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gzkdesbgd.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/glpydyszo.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmuvfxxbg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gxokhuwjv.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbtdxoomi.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gebhsnewi.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkslbcaf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkeuuvkz.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/glxtftkoj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gldiruikm.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gkqarrblt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gteigrkws.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrkshocq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmunwbljl.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/glzkjhvbp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxoekesh.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gwrjylwae.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/glhbqtzdn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvptngsb.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzhjaztr.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/guzedjhbn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhghgtzk.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/grppjgqod.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gsblcpaez.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmczazqjm.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgubwzvg.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqkooijyq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotdurnco.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gnfyfidsm.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gtazwhykj.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/getidxwrt.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzopvqp.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcxbxnbc.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/ggfmcjuoa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gonrjbqfs.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/glhudvwee.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquafdeca.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gtplilugh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/giyhfggrv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjmiubuf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjevcuhzp.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gauhejhuh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmitblsyo.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gprrbrllu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzcbckqp.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gwnpcvcjh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuokqnhf.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaeqwruw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gvjfsvwhm.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjdbsbvqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gasmxiyfs.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/ggsyjbxnu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqziaslv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grtleuygp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gumondhtz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghrgoqvln.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzihoaqdj.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gepetxsou.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gowmknbjr.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gghqjsmyf.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giskjzvek.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxldqrjs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvexoybwq.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmdgpqzf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxokwxej.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdvaxvkpa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuzrmbzj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwyuqfzr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaunljlyj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnpxidgli.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqzlzvzol.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/glwyomygh.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gliqeufgn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsfphtzk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzyycjep.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekllsurv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/glpsvarra.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gedsbxifi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtbwvuyy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ggnfrztwg.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gtevwjrev.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjdzwsqv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyjzbfif.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gidzbdoyi.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/ggbyyeila.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqenpekhb.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gmpqzkpme.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfsyivcp.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/guoqbddqb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnuojmej.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/grrmkuwkp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjhuxbo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gveofnryw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gappdfpdq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqgzsiff.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/ggsgmmgou.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxapcjfx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxxpwuvpm.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpihyhqb.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcugqcpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/goaghulwx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/ggxntxxnn.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/ggwvvsidb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhmrfvnn.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjufjmfa.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gpetthuyk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdsstpsj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ggxpyotkc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjreipdu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gfdwzksjd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gqujmrisy.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkltggjnc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gnmvvgnaf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqxldkdrb.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gwrqbylts.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjzgnym.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmevxjeqe.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwssctq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgwyllfa.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gvirbckhv.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gldsfulbz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gsetfsdom.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gljtbpgdr.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxkphqxbx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwatxejcx.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhayexaf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gecjhfpbu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrdleohc.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghltfifsw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkalevni.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gginfmqqd.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gszudlczh.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gsuxqdcwj.sHtML


<!-- 参考信息 -->