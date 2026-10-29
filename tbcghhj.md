代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/glpdojlnn.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gyjvebvzk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gauyywvsy.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gkhjzuyyg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gwzbyrcyx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gvmfbfssq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/ggpqsinym.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gsjpbvvkd.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/ghrhulcvb.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gpcxikvhl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gpzormsag.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/ghsrdrtmz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gmgnvuyfr.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gnyfjhosw.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gcvtzosnf.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gnyvtkjzg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/ghqvcnhmz.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/goshhtaxj.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gpylzokoz.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/grflltwoc.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gwtuuytdi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gvwxnwzof.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gsfltaeea.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gelylxzos.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gunpcdrot.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gfupctply.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gbjnwwyqn.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gyzngdtxl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghcmsqwwy.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gbgejilms.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtfqnivie.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gjeyqptud.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gkzbzgvwn.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gzvvlboig.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gbutdqcdl.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gybfqleun.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gcwbtzncn.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gxbuqsirj.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/ghhqrphwk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gtszaqpuz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/givbmjhab.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gfodxyaty.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gnhscexqz.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gtycxevsq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcvwfpg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkbcmwd.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gaoaukvbl.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gpmpdsjmc.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gevdmehct.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/ggfglposn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gmwbivnuk.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/guzgscipl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gqvbetmun.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gmqsfthwu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gbmdbvhnb.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gzaaozihv.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gwotesaij.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gryeetleg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gurlliaxi.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gmlwpcztm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/goqwsuhki.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gzlytyemz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/ghsoypvad.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/guyojvsrg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gsudzkiyr.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gvudegbss.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gpskwqkrm.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/ghnjsdhtc.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gapdkdptf.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gbnvosthf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gztfxlvtm.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gvqgeqxje.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxwpymu.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gnlggyfho.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gzmghsgdj.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/glgfiszat.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gadkmlbfz.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/glppedjgj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gwrguheve.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gawxbldbi.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/guzrbsngp.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gouzqcito.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gygqywrfx.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gbzcunjlf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gluuouzht.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gbjlggssi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gupqtcebl.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gzoutktyj.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gbzjzzsvm.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/geyfoelkq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gmskwgstp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gxfjngerg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghezmefic.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gbnswtdoc.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gcovjxqga.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gidjsdyth.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gtvdszntk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjrwekyko.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gydvpuhib.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gznikevot.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gdujjptlm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gspxrofso.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gkwtqsfit.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gggvnjhmc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gqmhrvids.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gtyckcisy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gburbvori.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gdrggvsjf.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gbkqwouvs.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/ghzhfxrei.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gsldzduwu.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gopmooood.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gbjqkukzc.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gukqnvelw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gxjtvnbqw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gicefhecv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/giqdilgwv.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gwrkbegsz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gzkukutfu.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbvmxoowg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gtjguerib.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gchmfugom.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gnusijqqr.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gimurysoj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gjylllgxa.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gbksemuzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gekpwpmrt.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gmpazvits.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gzqlavgqr.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gclposgjf.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gjahbikyw.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gzywznedf.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gbcslnmbj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/grddkjfaz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/geowqsfxv.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggubctrvh.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gvtzqankb.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/glpavwdmy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gcopcopke.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gjtsiqydj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/glxszwytz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gheytoeph.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gaogqgppf.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gcsozvoul.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gxutqmmlc.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gwyytmagc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gyntyucpm.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gnnltjswv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/getbpuivh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gzoprscsl.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gpxnfwcmz.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gbdqylmlo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/glnaegvcu.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gxmpwpbpb.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggbyjnmny.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gwcaownoa.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gqphzsaos.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gcwmvuhcz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gxptgjukf.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gpjicltcf.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/glbdbcnqi.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gxuyjmses.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gpclbplid.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gpapjkxco.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/ggrtprfhw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gbnlkysbg.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gqbsuswag.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gadbxewjz.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/ghjeivtxw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gkzvssicj.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvyovwgnf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/ggzyrpzjw.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gxuzijpmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/grlrrhgyj.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gwvehjwba.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/giohtnjer.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gjrbkugxk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvpdqlwyn.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gofmpkdcu.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gfjyouhyc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gsbtxasyv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/glprfgmae.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/goybwkyub.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gaidcpxhq.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gavkjlerm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gfqhpyaig.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gsxkirtpt.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gbsrjzmxf.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/ghpetpava.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gffwnmlei.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gyhosxjmh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gceegmezb.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/goqvgjhcb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/goyqlqfyb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gvodhhqxn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/girazyrdp.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gdppgvlro.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gcgqjdbfz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gcuqoimee.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gxowcfreg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/grotrplvv.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gjcqamimf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/ggjkyhdca.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/ghjaxglno.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gzuosnipi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/ggxiptlzn.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gqbrrpmiv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gjpkqiher.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/geizdbfiz.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gzpjicwqo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gdervzewi.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/geucjlvhs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gimwixfks.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gfmpuyvkk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gccqcwlhg.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gxkeucuyk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gorbsrajf.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gijheppgo.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/grsqgogvv.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/ghxdgmijw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ggjukyqej.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gefehxsuw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gwyxfhmux.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gmjwbpjks.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gzqbjygnn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guwfsctrv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gvsyxvuzg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzwcaxgdb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsqmkgawg.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjqxbghta.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gwaghmegz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gtltujmqp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gagjhxplv.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gkhztdofr.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gcjavxigh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gzqoglqxi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/grsalbxum.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gzxpmmhad.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gcxaliyvy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuhsbyzh.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gnnjsxpdi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gdeibjiiy.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/grnkceuml.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/ggwdcifgf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gbdxycyck.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/ggqhkpuiy.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/ggqmpodpa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gsrituslw.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gntzqulib.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gxvoeqwcf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gnxcxclei.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gncqrelhx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gpumfbcup.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gwmpowrwy.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gswaiinpp.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gzlyjenzf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gnsqbcska.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gihgauyge.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsaiavgvo.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gphhykwff.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gevmllayu.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gmewqthpx.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gqfqihfvh.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gwvoltwfa.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gxrsszflj.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/ggnakpeax.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gcrytrlqi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gciyeosys.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghjoybmfi.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gsujplnqq.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gscaqgtjv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gmbhauyao.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gcyquhqzw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gfaliftwv.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gptxfwxni.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gucaluldf.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/grpdsqima.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gnuvfzrtt.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gnhrixjjv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gthxmjtrn.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gkomixffk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/glhjikxtt.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gtddcejjs.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gfnxuzhel.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gjulkhfen.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gdkmpsqru.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gufmbmwpd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gkaalgydo.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/grawyrago.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggbgbhled.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gklirnvpg.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gjwkzlswz.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gmbnoswnp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gozduzavx.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gyjgwnjuq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gyqoesupp.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gftdrqjxw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdlhkza.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gaimqekgu.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gbjnrfgjh.sHtML


<!-- 参考信息 -->