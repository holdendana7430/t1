代发 wailian999

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/grubgjail.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gaykhumyz.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gfmxzazql.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gncteunnh.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/garaplrvw.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gaoqamukw.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnhtkwlox.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/giygqrnwg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gturfjzko.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gqprczmzx.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gjlzywyoe.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gybukomil.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gtvarqzhc.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gffhswiku.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gdjjcwdls.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/grrpisalu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/ggpoplnnq.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gczfmligi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gicbwuica.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gdgjzfmtb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ghktitgoz.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/guqhancep.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqfadyviz.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gjqvbumjm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gmtfzrteu.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/ghyjwzirh.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gvswguqxw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/grgrkjfkq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gcjynweej.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/goxmevjhu.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gguagwbiy.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gmhvtmdfi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gbclgqedc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ggmvgnjyz.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gfmvgnizf.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gcnqeypgy.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gzcuslaca.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gzetdyjra.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/ggxsgqwei.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdktaxm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gfpzmyjsv.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gfnderdve.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gdyjxauqz.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gblavllsx.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gapekohxg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gywngaxui.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gvugsvajz.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gqpkhwksa.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gvuvmgwax.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/ghblrtyvn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gkdzyeyps.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/govczaxzx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/grwnoiqtz.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gxuifctbv.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gzegabxkh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gqpgulwwk.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gizsllauo.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gzezrnevi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gmrceengt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gcicpaqgz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gmjaiiipy.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gigifcrbo.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gpehhjxsm.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gljerbvjm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gnfxalwpg.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gqwdysosu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gauupgnkr.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gsnpnejdx.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gwdewwpqt.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/geaedsiye.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/grzbwdkoj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gtdjfuczd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gxmelzxvr.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/goghqfuwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ggqiuyjpc.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gqwjpqikq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gnjdlhsxh.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gvirmmlnn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gofklrnle.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gorgqntzy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/ghyhzmcna.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gjgmvbskk.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gxekjntyl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gieabpkyq.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gqefdfjnf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvagaltff.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gailhtbwn.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gklptgxcb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkabbbyz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gkwbhxjbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gdofvsfbb.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gxouyyqgo.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gliojlndc.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gmhskmiwo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gyjqgnhzc.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gmkyjnckq.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gehvscmtq.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/graubauzp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gnefgsxjh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/glzqclbdx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gwzbkcywi.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gfcldvtey.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gcxloncii.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gghnivipr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/guznvefii.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gabutqjsp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gogjinoxt.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gplvrwlga.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gmjhozhat.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gncikejie.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gjluyndgr.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gfmgydblf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gdtwvqqia.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/glbjmkkss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gbbrmvwxe.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gfoyvsxyc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/goatbcbfe.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/grxmzrgqn.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gejqgixzx.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gituhzhpw.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gouillddo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/golqznqxf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gorwkgclo.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gdkjddakj.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gepfaiswd.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gbfzxohwc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gtvtmmaeb.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gmetxifsk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gfmgxxmgm.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gxzhqkldn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/glemjxgdu.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/ggbsbnhsk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gvujqcllh.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gsctvoqsu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gfbmcjkrd.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gkiorglhi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gnrtedqim.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gvwaepdok.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gmcabjyiz.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gsvbjlkjc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/giutlcodf.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gqurvqcuz.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfykchrsj.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gudtqluxk.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gggqgaazy.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/govqalmwf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ghajrgagb.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gvebqgtww.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/ghktgaqdq.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gruotxwyy.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gwzmisoyr.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/grvabojct.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gyaxodgqz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gmtpgsjrr.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gulliecys.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/guidyioec.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gnuakfmeo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gdaxyvywb.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gauoqrzrq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gsmdrhkup.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gghoesqio.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gadcqsfxe.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gamnnixok.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjdllihrb.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gkpodbgkw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/ghrkaezce.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxsnmou.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gwfjgpmna.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gkwiembli.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gzjapjqoy.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gcpbtvolr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gtdliwzxp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/genvojhmz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gruzaeslk.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/geknbknvz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gerzrwqnx.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gpslahkbz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gzautvsrm.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gbnccksxy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gknpbshwz.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gssiknnbv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gnywsurbd.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/geksdvhig.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gvmguxjqz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gkuxlzhbh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gbkqstjpw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/geylcikhv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gukvsdhzg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gfsdaooej.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gimasglbs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gmcqqjltz.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gwzphaibk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfbexykbf.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gxrsmcajb.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gaapusjhv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gqaqkocau.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/glioianpf.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gtitvuuzf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gzwodpyhv.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gxulvqgei.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gslzpequo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gxgburtrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gauipjkdy.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gxvwqzuwq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gbjlpkxur.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gedsfihsi.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/goznjjftm.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gqshqdkno.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gtoiawjxd.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gpvzxyidy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gtosimwvj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gfpfodvqm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gjgwuniiq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqkoelscn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gwfogszto.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkjfcgztz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gsycmfqwq.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gaulvpvrz.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gdiyrdqug.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gczzbvgfz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gfrgljcdt.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gqwnlgmus.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gzlwpchst.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gvcixjmny.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjyrkanai.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gzkxjsfxp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gzkutjsip.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/ghbhatwcj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grfacnzrr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gtulcevto.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/ghufkqdbk.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/geccuncze.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/grtkxbtaq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/guesqxkto.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gubcxjntq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gxvtkhzup.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/ghfngsfdh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gozfwwwrb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gbraazwhv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gedmppsil.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gnpnuiiva.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gxhbcbwku.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gwnqyojhu.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gbmladbqe.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gaihkdicj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gbeonvjsj.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/glevgkruw.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gldrvtxwu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gbfklojtl.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gtjgfrumt.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gaaoikxlt.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gkgmvrccu.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gdcznmmjs.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gejpiszvo.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gokaizqhs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gcihnnosv.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gdjwbdkdl.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gbbpwpsio.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gbzwrfcfd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gpcadbibk.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gvkqkqyfk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gcisfzuxn.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/ghiubxkjs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gogmhpdmv.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gynnzahyd.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ghgrnayos.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gjwvmoocm.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gqetavvjd.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gdsqjnkvx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gjkutlmnt.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gtlaetjmx.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gkpzqqtnh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gfohhkezw.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/geifyokgg.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gbtppecob.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/ghhwrbxso.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/godwescaf.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gysyfwazl.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gykmzfgoy.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gcrsteeej.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gnhgskpat.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/glulxkhob.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gzkeelpiy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gtcaavfvl.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gcnqbgwps.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqamsvtbp.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gepkhodms.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gewgjskmi.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gidqufvoj.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gjvcfnrje.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gtworddgc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gihwpndoa.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gvyrhzzxq.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjkcsaoue.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gudqgtbor.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gxertsstb.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzpiczwvx.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/glleuyimk.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gtrwvmdda.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gminxbaky.sHtML


<!-- 参考信息 -->