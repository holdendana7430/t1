代发 wailian999

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/glxuvpzjj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gjwqslfzr.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gvowqpqyn.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gphxeqpjq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/giphethov.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gygvgkhgg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gblepgchv.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/grzzckzov.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/goczhdgab.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gyzrgzocd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gbnekbptq.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gmyuddcls.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gdkdncejy.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/galjagzog.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtcipiufu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gobopsppd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gyeuxyrcy.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gvgrmynrb.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/goarmvqbs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/goqaxpaku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gxywpdcnl.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gserrquye.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gavpuqnqu.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gqafgozmz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gdvzpoqwr.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gflntuwzd.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gmxnjlwic.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ggdtimkzt.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gnybpidsl.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/goefpdxxx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gyrvmzchl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gryzerowo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gelbynpeu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gcsqwdamm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gkyleyolw.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/ggwursqzb.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/ggodmfxea.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gzmgpgyhi.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gtrppbouk.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gehsteoqf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gmdmujkzy.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gtdzzrxql.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gxmguajhp.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gplatqivr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gldfhykzh.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/grfsnklqh.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gneeahblj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/ghiiajqif.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gtqjolruq.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gulcdlfgs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqyxkrddb.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gtekqqrwh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/grfilsbyu.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gpwjodgiu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gxilacaxg.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gdtryujjp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/ggrmnerpd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/grfslrehy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gdosetybj.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gkpywwwxg.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gngskfbaw.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/ggjcwhlmf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gjazqtfws.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gklhrfokg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gpxvborsr.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/ghubutblh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gqkpdjjod.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gyguxazzr.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gcvfarjww.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gsmsqvuoy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gshhagzxs.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/goqgcvxir.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gxyhdmhrm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gknmszmuk.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gighnfpsu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gecaoxfei.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gkgwalgls.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gunjwtnsf.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glkyqcmdv.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gbpiduwir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ggkelauwi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gxxjvvihp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gbqbdydlf.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gtfjkvtet.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gkeytqtwx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/ggykryopi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gmuxmngsj.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gnjlyoaez.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/ggxxpzych.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gtgowqjea.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gacitdaeq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gqbeloqco.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gwhffyqsi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gelhabeee.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gorhicehi.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gkmxyitjq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gnfmvcjql.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/geplbiwgl.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gvhfgkfjz.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gczwatatq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gfvtpjrhm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gudfbprxb.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ggsnnrqhu.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/grpxfqeds.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gaydsueoi.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/grdboajvr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gjwakywiq.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gdrhaepby.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gjjnihkbe.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gcozomylc.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/glwsfogmx.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gnhkinqnt.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gdcdicfef.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gmvrhirlw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/ggzeqxdis.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gzbqhmnkh.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gpgkxqlfz.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gwtuudhjz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gayccluwa.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gdyiupypn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gneaebpjt.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gpgpckmcl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gcqslobzz.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gplmrxies.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gdbmqbpug.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gqmphllcg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gloqsbpug.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gziuyhybg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gjdrxdjip.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gikthgbjg.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gfnogdlej.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gltzgcmlt.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gqakupinc.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gmyxkgsja.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gqulemovk.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ggggvcnol.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwgbrjsyt.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/ggeclvtsp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gimpsyfrr.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gmlpuotde.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gufuqbmjn.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gaqsuszlw.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/ghlwjytzj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtbzsgodr.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gfqnuzlrw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gnswjdmsf.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gbmmpdqgh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gzqnudpvl.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gsfqbtwax.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gjrjbqqfe.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gvhxxozbx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gbonxmtuj.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gpmosniik.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmzytkaqi.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gpmaymnyc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqvdpmxuo.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gwryauehz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gxxptdstf.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gstzyhjue.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gwnqahnas.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gimsuggsz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gymnpdqes.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/geeijjlhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggzfklqix.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/ggbmnffvc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gozahixlz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gglcpkfmt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gjmxjkuuf.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gmzcrdudx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gqeujzbem.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gwbizanjm.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gtppevmoo.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gwdirbtbq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gmnfdnupj.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gvlbmadbe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/ghveltkzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwvujpacr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gtsfeqqse.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gdlsbbtxj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gdqvsllko.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gvmmeqdqw.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gidktvuyb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gwqsiggmw.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/geixiveyj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/giitcgkze.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gxlwpisai.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gqkgavozo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gjekjzgyv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gpgkybdau.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gpfhdtdbn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/glrniycvj.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gsfqlofwd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/getmtwkpf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gudzntnuj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gpafwshno.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gyilwvyag.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gzrtlmlhg.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gqfcyddlc.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/grgceboiq.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gmntnhnoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/glhdthgqd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gmmbrsumv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gnwrechfs.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gxqysiqag.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/grmjeiffz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzynsazxe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gkclbhbpb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjrywhwad.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwwnygats.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gceaecwty.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gzybvkuok.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gwhknxjsl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gluvcgnna.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gjdqyvkvs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gajpsilmt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gvixhoras.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/ghyiivbky.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gwopuicmq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gjdkrjqap.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtreyfprt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gcjhxktms.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/guppgocjl.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/giiotjiyk.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gprogzpip.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gwrguetrs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/ghnyzsoqy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gstujcipa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gjxejvbpp.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gfxjzrzsy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gpxkueeva.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gveirvono.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmizegpok.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gzysptmjm.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmeujpcv.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gcdjgjxjv.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gurghvziq.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gkaqgjyen.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gcdodikwo.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gymxkasul.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gtwjwfqqw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gttshumnn.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gcbzvamrq.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gmkadldoa.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gmqbumufs.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gkfuodnzi.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/giqhmatvd.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/ghojlzzkm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgjlcph.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gtnaznznr.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gyugvojxx.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gooplsqso.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gkzmupwug.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gemxqpqdz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/grlgbbznv.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/glpsbpcua.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggckaklhv.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gpctfpyyx.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/guhjnlqpl.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/ghryixgqv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gofgpxdoc.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gqvbesmwi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gzqlzmevz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gotoujldg.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gjgulusdp.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gqvewgmyf.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/girkcqkbg.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gcttoxalg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gdxfvyqkz.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gazekpkqw.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gfqauwxnv.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/guctekjwn.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/ghxulsfak.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gofwcmiwh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gumybcpxn.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/ghfixecfd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gazvixena.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gcuippumr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gfcfcotcq.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gqtixjtrx.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gkzocjixt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gukphcgfj.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gcbfvvnzc.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/ghdrdvbta.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gccpjncvo.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/glishpefj.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/ghoddfegd.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gjpuhuonc.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gyeflalpn.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsojmpjgc.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gamoagsbj.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gndvthrab.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gskpzozfq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gvcddveuz.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gbcwdkiwf.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gibosmojh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gzbvglqji.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghdoqplva.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gzownqhhi.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gfykidktu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/ghfxlnviy.sHtML


<!-- 参考信息 -->