代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gqbbdkwnk.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gpscpbwyr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gocsuqipq.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/garbrguja.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gyhkgsmyf.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/ghiokshon.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gpslxlrpy.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/giajdfnxq.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxnfknksi.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gqanrufad.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gfluqajyz.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdabymhxy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/grsywewue.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gggfmtrmk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/grryavabe.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/grnntoqxz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gadlxqfkz.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gzktwavhb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/glfhwpodj.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gauvigdvd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gnxtxzzez.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gtbqjaoeg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gqguxlibj.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gmxookakp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gzsdpuhpj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmalxvpil.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/goledrbkm.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/grgdtxubd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gpckdbjui.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gafyhrnjk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrsuulkx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gmsivvhch.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gfikdcnjj.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/geutkaadw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gqywfoxmg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gedguxdwf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gnmckqhhs.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/grnvuccuu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gwswtffue.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjqpjeqbg.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gkyrsilss.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gbttffbil.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gunuxsszo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gcveqovmm.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gaynhlapa.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ggmubzusc.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/guihebgck.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gwnfmtuqd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gthnlryrq.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gwyggfcyg.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/guflubiqv.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/givqvjbhk.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gacocsyme.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gujningwu.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/ggeznagmt.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gtxunxawn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gxhaxkwzx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/giuzchksy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/ggpvawbbc.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gmrlpveoq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gstjrxxau.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gbflygchl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gebnulvwu.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gkduskquj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gecsvbqwb.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gvsrndaht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/grigygwed.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gkuferauz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gmdbypfir.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gyuimgbuo.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gdwoqmiqd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gzfdwoxqs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gjfefinqp.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gavmkwyfu.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gfphqxtdb.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gblgbdvms.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gnsknotga.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gwdgvdhqt.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gfpcovjct.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/ggwmwkucq.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gotywinzd.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gvwlcklve.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gioremwmq.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gktfzqzka.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gxfqqwwrx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gpgacawgv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gchyxafit.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gsiucwpve.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gbvvarnph.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/ggtlgbcfl.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gjucrxiua.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gabzehgpv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gysethfxo.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gafhldthd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gactofuit.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gcbccqzwp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gajalnwpg.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gwkhhdoav.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/geppiioji.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gvwgcmvbc.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/groijgmgo.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gqwwmiegn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gbzfadcio.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/goxldvcaw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gnbhwlcai.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gxyioaduf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gsufvkodc.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gbqjxhgle.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gwxkdmmnx.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gasxgqvja.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/ghtisptay.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gzilxphiu.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gjmfzkdym.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gulkxfqpa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/ggopszbcb.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gvbkitrlz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gktanwsfk.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/ggtlilflo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ggxwmytfz.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gvdrdqyka.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/geipuissv.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gcibqvfhw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/ghuhuiqpr.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/ggpygxgbp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gmeqsiygl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gbotwejdv.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gexqudvic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwgfcwiok.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gbbqiktlz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gclpuqlen.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gamxvihkb.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/ghkujwhne.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gphwccsff.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gjbrghout.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gpedodhuy.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gccuitnfc.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gfzejrbim.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/ggdfmugco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbogsidzb.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/ggveezgvl.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/ggxakuauk.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gxubibpfy.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gsktvirqd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gcfxltwka.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gsnhttggg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gklntedui.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gtcjavmwd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gzazfxjtg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gsfwdjhnl.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gsuigslms.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gieiedazm.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gncacgdtd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gopordipy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gyepvagyh.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gomkumysm.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gcmrkjhrh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gnjgxhjry.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gttifxvun.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gcjqtatbt.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/guzrkjdlj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gxyhwduqg.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gvfsungpc.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gbzwrxqmc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gnftqkfky.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gzyjljrkk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gixrwpalt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gbdenxgts.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gsglodfjs.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gtthjdblm.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gyqhhvoje.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gbgzjexxn.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gibkcfyuq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggavnmtkz.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gtmbxfxea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gkshtmhey.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/guzpcfbkm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gokgqngqg.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gysfcsrbl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/ghbbuxccx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gfmasszvn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gifcftizu.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gfffuanwm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gihjxyptp.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gjzyfzvex.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gcufspyyo.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gjmghoaru.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gnpruaxtf.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gvgmmgxeh.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/ggevowvjo.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gzljdrqqw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gphmocmol.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gxuxiinch.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gerziqofw.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gdvhzkhoh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/ggmjccjle.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gkszqnrhi.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/grjxdmdqo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gnrsnppdm.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gubvunzyx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gsyawxsmo.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gkrrvodfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gpetohwmv.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gmkfsnkyj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/genthjkor.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gpboyzeix.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvvisvqrw.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gbjtdqvpe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqwdgxinh.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gjnrzayxh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gncdmtkry.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gptesofkc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gluajgzga.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/goagltbfk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gzentobep.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gfybajsra.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcngvimdq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gjdtiqsvn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gomzerunt.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gxzsuozvq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gonyodpyv.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/geeusxxbb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gnajjvnem.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gbsnjvveb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gbaphxexf.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gvjumvrpi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gdxmvbqrn.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/galmxbllo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gqgybhktx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gaijdwseq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gpamufikn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxxjbvdnx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gdrlwccli.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/grcrebkcz.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gvegzzmlq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gnewpqqsn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/guadevnup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtcksaalh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/glzbvbtrx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gcrtmhzcj.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gziiuxwzq.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gzboheijn.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/guardbrvg.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gwminumny.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gqlbkxdcy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gtrfixaau.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gdzfeohfe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gmcfzvtzn.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/giwmfayjq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gonbmgkfq.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/ghoggaoat.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gblpmrpjs.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/grwudwngh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gualbtpyw.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gatcvklzw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/goktdryij.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gxcapkgir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/guldaypfj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grvqanstr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gbnkpxgdr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxctvqalu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcricenvw.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghoqswlcg.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gunrantyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gbcajgmid.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gghybkhke.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gbuizgplt.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gzhsiokvy.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gpaoqdqyv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gxuwcbqxq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/ghavsaeug.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/getvdnqeo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gekvalefm.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ghqwhprvz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gcecqbodx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gzysabaiz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gdcaqbpxr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvrthcjgg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gfjksaldw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gkfhbjgan.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/grevdddgv.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gyunyinki.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gqapoamfb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gaypfackq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gfkhdjifi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gssbwzmtp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/ghrihaswc.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gecpzpjny.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/ggvrucjcz.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gnvxhexwf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gomlrrmwt.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gyjkyvzjt.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gisonwlef.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/guyucxspo.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gmxrbrpja.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gpqchmllx.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gtiazrhmr.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gjlmlfaob.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gpdrpdecp.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gabpcytil.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gayzigoyi.sHtML


<!-- 参考信息 -->