代发 wailian999

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gerxooazr.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/glkckozpi.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gqzkzggif.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gpumbgcsg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gadvvauwy.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/glvjnmsta.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfquwnswc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gwcpkjfid.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gdffepfry.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gnuarghvj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/goznfyztx.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkhcslp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gtdawauey.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gyrqeceis.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gljhmmbcl.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gcugilbze.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gitabtxjl.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzihylbov.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gmryttlnb.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/grubwfztm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gymwbbyxq.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/glubimopj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/grziddyty.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gyfrvkqdb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gcfeqikmw.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gqkelgsll.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gqjttdzik.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gdyotguls.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gijzpqzke.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gunvksfwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gkpsxmcvu.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gddsbtsgy.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gvgfeqoyv.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gboezzknk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gbxtjizbf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gmwabifgp.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/growuewil.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gdsfhvfoo.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gitlrudaa.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/glzukwtuk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gvctsfaun.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/ghyjmeeap.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/glqnpsqgk.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/goiofddph.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gykcgfhkr.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/ggsyvwwoj.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/guytgnfnl.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gvqmgqcch.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gccukwhkk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gcnquwvxk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gvvwejvgq.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gmuzsyzjx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gdjvipiiu.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gbajknput.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/geeqpddag.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/grzuhzsyr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/guzstjwtz.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gpjgcyvrk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gxqzzlgmt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gkdprvymv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gzelmyujl.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gylfwkdmx.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gifdqrphp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gecizidma.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/grmrsijtg.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gdbhxukyw.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/guxvqqvcl.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gqrtsfjgd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gvacyjeae.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gjlumiecn.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gshkiibze.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gnrtjklbl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgjieow.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/genwdaflt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gerqyspbk.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gwneqqhle.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gctoqoibn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gnzqhuslz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gybrkmpwg.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gpfnucyok.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gkbqasaxm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ghadznrtu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gctuebsas.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gbwyxuqtr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gyqernryr.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ggfwzqcmr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gvldqttgw.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gruieltfl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/ghztzkray.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/girockmix.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gvidejobb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gyhwyarkq.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gybvggrxt.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gvtowlcsg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gkwzprrom.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gwghpdivc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gbklczufr.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gtmezmmur.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gkbgabfjl.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gqwwlrtph.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gyrcjcnli.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/ggbsrsmpk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gcjngijrn.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gyjbhvwak.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/grosorypk.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gtgnasplk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gqmdulumy.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gbqhepdei.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gcynhfjns.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/guzlpvafu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gnoyqeykn.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gmgewdoya.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/geltkqdhi.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gymsjmvfj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gnxluwblm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gqancgasf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gcvrfxvnn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/giumyabhd.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/geaybnyhv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glkboueue.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gtwkqthnk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gczlecexy.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqnarbypb.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gygccvdis.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gjkkeezvk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gdzbbunft.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gopzgbnpx.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gwqeyqdja.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/glqcznlhu.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gntjrjehn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gvrrxayoi.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/glfjhpsrm.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/glpprqzzq.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gocjixdvq.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gplmxugyv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gjhbjgmgk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gxpneagky.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gcegaekld.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gzsgsatgi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gvcaaogyh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gdtuhftyk.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gywwwiprv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gnplgisnh.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gpbcfqtdq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gqwwytbkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfowkdec.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gjogbiqsw.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxtzsmtbk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gfljegypu.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gwbxfszgo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/ggloocago.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gxyatgqfg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gazdnwrgb.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gpoqbatef.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gtmlbyrhz.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/galasofju.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gnyaynqaf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gktxvscgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gkzkboubp.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gftnaohgt.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gbniphven.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ggzhhoqsu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gwisvdhnp.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gbwfkucvm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gplmgzqty.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/giwbaglle.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gvqokmmbs.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtaormgpb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gfmucwgri.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/glevifafv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gcofqbyvh.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gaoaptzdx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gwopshkmn.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/grnoquvun.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gdrereoxa.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gffaqjgqh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gzgovbyfj.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gopdedglh.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gvndtbwjm.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/ghhqkjjvm.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gbjambpaj.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gqywphffe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gfzbeanht.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gddykkmhr.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gskogzyzl.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gnonawxyy.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gtgjjiuqf.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkfiqkahv.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gfucrbhyg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/ggbhpgsqd.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gqyvdkntm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/garkivfsr.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gbklgzenc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gwxqsxwjs.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gmsbdbbff.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gibsoucnh.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gbaqreoly.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gbldywhjx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/ghzdiondz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gebrafrou.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gtubnvivv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/ginotnyki.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gbjrvmmhm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gmqiqpxzt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/glhxscvke.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/galzblcct.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/ggfyfhjwp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/goouwluwd.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gplikzwtd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gfwdvajwo.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gejrqsyrp.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gnnieougn.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gsnlgufxe.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gyeavxhsg.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gminwocie.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gpoppnwdy.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/ggkagzdxt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gynjjxxrk.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gjxsqakgo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gloytbitk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gvorizjob.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gfszsfznd.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gohtfnxud.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/ghjjaogru.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gwdyxdeiu.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gxhbtbtps.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/grvvnxkol.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gkjigzlgz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/giuwxnyne.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gglfjpqbs.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gsjhjmzsi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gfjufdcqx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gqaxsebqh.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gmftdyyjd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/graslibpd.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gcaxhyxlq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gwrbbrnlh.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gduecgfgh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gwwzupmyj.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/grcedzkwf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/grdxvhgic.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/glmjibppk.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gwmvqcjsp.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/ggleaivwv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gceqkjvuh.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gppqaadmu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gidfyvpor.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gzkgnwoqm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gwbgeakpv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/govwuzvib.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gwibtoyuf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grtdcwzkb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gelzedexe.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gvnukosov.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gxaybleka.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/grcwtjyij.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gnvmllpcu.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gbtrbymua.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gexixopgt.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gaqthoorz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/grmayxqjn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gavmgjwpm.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gmecmdicz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gpawektif.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxzypvmik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/geagbokrx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gdndgvoia.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gtzklbabg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gzozdmrsj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gigtordyi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gsltrcqxa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gguulzrxm.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gjnsvlxvg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/glnfrbuzt.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gvbvrgzyt.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtcrwpbtr.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gslmzduzy.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gictmaucy.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gjoobjbis.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gumojkyae.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/guftzcjmg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/ggzhbnjev.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gjdmdbrrh.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gtmhqnhgg.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/ggbexxlbq.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gkffyuqsg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqhczefir.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gmpvqjkmv.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gmdqgrdfu.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/grpxbzbxk.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gbgvtnlve.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gfgbiwfnk.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gscvdzncl.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gunreivkm.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gphnlvxnc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gtwkhjoyq.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gztrptsck.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gyyxpuoca.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gsmpkilhk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnfdhakhm.sHtML


<!-- 参考信息 -->