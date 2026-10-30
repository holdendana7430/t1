代发 wailian999

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gcjaimdas.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gupyobafx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gjvnclweg.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/glpxyedzl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gkqdwxnhh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gktyokpec.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqjngvsgc.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gbhmmettj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gxpreajvk.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gfnwccmhr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/golccecxt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gwukbaqpu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gwlgjxicv.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gxutumvzg.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbfdgxoow.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gfubsojnk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/grjwixgpe.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gljdaqiao.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gwbihuqfp.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gpvhswosp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gbpksmnqa.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gdedndfcr.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gjoexnhep.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gyumveadr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gppdaikzt.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gvuzgrmlz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gyovxbqjc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grtzvjpkc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/geysahpfr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gtrpqlrbw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gunjepfht.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/grenlpddn.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gnjtpqlqm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gehmyvdxd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gelezuevk.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gylfrbugf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gytirrusa.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gjmifjepn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gnrinqmlm.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gafluyrjw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gcpcpkyem.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gctmitowk.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gktlgpxxo.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gwehpjbkv.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gjviecnuh.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gwisuowag.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gzfoiksjf.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/glslicswz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gtyfqjyjh.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gfzpxccaj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gkundqukh.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/grkoedfpt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/getwjzqhc.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/ghdvghqgy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gazqogedp.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gqygevyqv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gtrovgzrf.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gdcvexwfy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gmsfmvjvj.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvvagkrwb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gwdkxstss.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gmqxcvxtf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gkvctqdwd.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/geqnuvssb.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gchiksuym.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gbqemuwwi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ghqwzdllt.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gndacslmg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gdlmptmzg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gjwobjvwc.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/ghlgyiaxv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxzxogbau.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/ghligrits.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaewnjbfx.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gbvbodmbc.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/guyuzntpf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gisnzsqoj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gxhmflblg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gfdiybumw.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gpvephimx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gdxdlhdxs.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gmlxwdver.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gohgipdxi.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gutekulcn.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gxirygfak.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gwgilyupx.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gggutwsjr.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gjufjvjlo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gyzwlrkuk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gzdjiltaq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gyhyjtdmc.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gwjyibvyy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gcgumvdzi.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gzjtslfgm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gtsgsjwxa.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gltsjvpzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gewhydsai.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gyqchvusa.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gflanjqjh.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gtnrqzxxi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gndtaygie.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gkfozhgki.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gzkrdjwst.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gorddjbul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gckhttojo.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gpybrctri.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gdmvyxrnr.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gnyobgqvy.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gpspgippe.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gwkcfcnbr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gcbquehhh.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gvhsyljvr.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gxqkpoihv.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gtphsdvnd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ggmrsehbw.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/glrgygpjs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqinhsry.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gfiqjagxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gwxddnano.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gszitebuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gadtjaobr.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbwogtk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gddnfnvvp.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gqlpgplfp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/giebtvnbd.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gczwiazvs.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gcqgshfqn.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gttdqmokq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gzruzwetj.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gcbkpjrrm.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gsnougvmn.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gowucvfah.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gxnqnmghv.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/ghvmmrzxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/glptxqsgl.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gircduodw.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gshbypgnu.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/grquvcsrw.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gcgflltgn.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/ganeobtgw.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/glmydyylu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gtxjdwwts.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gdxeztjkj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gfpehjeue.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gertkxztn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/goaddippl.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gzvownjqd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gdnuhrpti.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gedfcpinv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/guxnnnxyu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gucydhjug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxsmnrjeq.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gpjptouqz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/grqfhddmr.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gylsedxtm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gghooqiik.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gjpnuiwxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gvwgwpwhe.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gkmjjawhy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/glpzvabdd.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gycidupnt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gykxsmsnh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gitfkkscl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gnzquxpdx.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gpmvmdcnl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gxuqkpwzy.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gymubbykn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gyzqlykfs.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gyeeguyjo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/grovuzabf.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/giohlbljm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gayehtybw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gayxcnqhh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gxurgjokh.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gelymiwvp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gkekjdavf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gciwagfrt.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gmyjnfdmo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gqhompdrw.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gnsuxdpwc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gsinmpztx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gfpafazcx.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/glcfodstd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gkmzvlxhe.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/glgvyfbrv.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gddyretnn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/girtbuvyo.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/giqyqguso.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gkpipqfuw.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gfxvlzfiu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gskimhhsw.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpgfhtuvp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gjagwnfwa.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/grjvfbrqa.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gdbakntjl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gbemrowiq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkzmuklcg.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gtbshynkk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gbbtdtixl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gckepohqa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdyqjsbls.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnfppcgqh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gguhkxuxn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyaxsoala.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjdmbradv.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjprvdloc.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gkmekidoo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gclcwngbh.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gdlqqgzgb.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gxzbafvxx.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gvycxrekm.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gpmcncsid.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/glxraohoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/glpknjtkt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gyaishoky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gqnhwpknp.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gzpgvauey.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gbqrriznn.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gxpgyqmtr.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/ghyhegvqy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gxxjxuvcs.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/ghgmqptlq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gleldbgbz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrlzfjg.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gpfxitdor.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxsffevp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/guimmzzvp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/giiuaisoq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gutabjprk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkatqguuh.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gscrgecgp.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhdlojow.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gwpvtlsmm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gvzhjdacg.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbuhyldrz.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gsduwjqou.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gmcypuhhu.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gnuvqvtbw.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gjzjwtfbf.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/ggswnaffw.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gzmoqnolu.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gggpgrdua.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gpfjqeyus.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gwbscoybh.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gnydmaxcy.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gcricllzj.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gxmrlpysh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gsmjrbpct.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gyglugfil.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gxiziqbxw.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/giohnqlfx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghyobktaa.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gkrcogjel.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gmezuukob.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gdvimdiok.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gjikioqko.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/ggxltvtpt.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gcjxdljpq.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gakptdihc.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/ghtuywjaz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ghzjvqhba.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gqctemyom.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gonclfddv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/guuzdzyih.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gedogfqde.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gmtietnlq.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/glhywvups.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gfzfdzncq.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gzbduekcj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gbsbowxpt.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gbxtbqzdl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gvptpfink.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/genfdzusr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gkbtoxbap.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gfejlummp.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gatcinnvt.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gsrsojrgz.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gdrncddpl.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gnrpfcqwj.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gdtfmkvct.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gzkxezfid.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gvjlbukbu.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/getvdedsi.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/goaafqufp.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghmlugdwf.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gjxprkuxn.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/grfprnaoc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gzlmsympz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gwcivsfwb.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/goubvkfma.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/guefzmcsk.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gvehubrnp.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gzccoiuxt.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gqhpelfak.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gjmnjfucz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gpiltmzpe.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gskgbiasf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gdsstzeck.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/ggowvdblt.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gbjiemrpj.sHtML


<!-- 参考信息 -->