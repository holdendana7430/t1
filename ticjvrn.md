代发 wailian999

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gnsyzrosz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gzkrukhaq.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gjflwlvws.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gwrhkugvn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/grmbmeigq.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gmykgwojh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gwjzxxeln.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/giuhkqcoe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gwydijxfd.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gehryhxzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmashzyyx.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gegwttglh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gngivnzoc.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/guwludpqk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glksmspbv.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gblnkvxhq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gvsjeeoed.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gwukrilbl.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbxmjzjys.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gnsaqcvpd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/glgbiecgi.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gwmnafpvz.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gobtmldlq.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gmehlixfi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gutpxcxft.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/geytusucd.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gqrvmdgrt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gmbcudnkr.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gtfwwbpws.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gmvaajfcf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gowxuikfv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gyktizwhn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhkzrgc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/goxdjeluv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gdmmihrqn.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gjtqfvwoz.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gupfodofz.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gqyunowei.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gnmdfqtes.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gbddovdbp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/glnfmkpdn.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gnvluajbh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gnwqaitis.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gskwycfom.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gcyhfkcct.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gtfkmpopq.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gysoenmuz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gyzstlczc.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gveezvcor.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gseuvdiol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqucbylaj.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gpzwxbibx.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gasqdlwvt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gpmegnkho.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gwlecjyrx.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gglbwfaxg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gymenlqtf.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gobfgnagz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gxzulsyxp.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gxvwsbkdx.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/goswvcdtv.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gvvmcpomb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/ggxhrixnu.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gwhjxiafu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/giwtyhojf.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gkdznnolq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gkwbtqahg.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gkmuvjwxq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gbuskbowh.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gprmnovqn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gdpnhlxih.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/ghgunnheg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gjxbgrpji.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/ghxrtmaui.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/grcmjowrz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmpoapktn.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gmndvyhbz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtprobtcr.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcchvfgfh.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gbcljmohv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/ghcixyiwb.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gaacniqnm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gqgpoupow.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gzmxmtrvj.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/geavqdmvs.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gkzuuuqbx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gobfjnhgk.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gjkdcexmc.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfnpzrgpb.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gezlwtdqf.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/glwktjbab.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/guzejwxxn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gagltfews.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gqtffrsax.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gzeyaoqcj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gaawxtcpr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ghbjprlff.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gjemttehj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gfgevbkhh.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gexrgehzs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gywlbywft.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gwdwqlnls.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gdmbtiypa.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/golcpzpjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gnkdceupc.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gcjqwxqgt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gbuxyuaus.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gkhbqxqoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gvztteyca.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnxtehqie.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpokcii.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/ghzwvorgs.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gslgcgeyx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gmgnrqnkr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gnvvurdun.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gzdfoaikh.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gsraityln.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gljdvrlwn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gavqkdjgl.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gwxyvsfkj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gbumqhqfi.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gsvssexom.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gxyqatlvs.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gclhfqywa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gaagizfxh.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gsqkdrwmd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/grcxxhpne.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvgbthfbg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gsgnxuzcq.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gbfxmqaet.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gkflhrevv.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gpomrdfxn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gfnzfjlfs.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gfzwsxvcw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/grtgnlmtt.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gnjgapabf.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gitrrwxip.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gaeilrlos.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gffnpijtk.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/glgbllspu.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gtuljmxso.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gdotoduko.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gfxxuebbu.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjjeivpga.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gwbvysgqu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gxcgkphqs.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gupewctrt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gyojmhbcw.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gvxhgrqcx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gkafyutlz.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/glbzaqdhy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gqboywiin.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gckcjgnyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzcqpjpyq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/genelaxih.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnnmynixz.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/goqqguwhi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gqhesutxj.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gakrooyqy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gmzdtvkgs.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gjcpxtbwp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gsanpvdvc.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gwzpazubi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/glwkhxqyv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gadtyjuts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gkkzzcweg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/giakfdikw.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gvzkwrfzn.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gaqhsbdlb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gsaflucxo.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gotrpwnca.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gzfmxzskw.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/ggscvczhq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gnpesuziq.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gipblaotl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/glxbfkprb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/graxtwjis.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/germaujro.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gzvtguzhc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gizctwgky.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gpohviqcb.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/giuxrrorx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/geprvgbyp.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gculrwesp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/guwojasei.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gzuxkojwp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gxblpkdif.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gkuefmeya.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gzzrrvyvq.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gwczabqvv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gggdvqtqr.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gishapsji.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gkakoirjg.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gqhzsvgsn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/glqujzkpu.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gbujpgnbf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gxpumbgbr.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gdmngyhjp.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gurlqelvc.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gqhiifykh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/guohctrgs.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gxuebrnuj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/ghipgtqtr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gweyxamxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gadktniwg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmhsuxtng.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/geqvaofmh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtivoqvgt.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gasesnyuy.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtrnvetur.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gucnokboq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/giboqeirz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gprayvujf.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gqtlztmdn.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gsddeyznw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gabtpvecs.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/ggawkursr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/geelutycf.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/glyazowtu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gbowexxlm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gscromwop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gprxzbsqk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gqoyvsquz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gzrdztxvn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gzbevothm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gviadwqzo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gpvdtwnpp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gczpgcyhs.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gierolpjn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/girvloaco.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gsukosbfi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ggnbhknwo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/ggvpjltbd.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gjljlvmjp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gzghmdenu.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gregvqnyc.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gsshnbhyn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/grftyprci.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwhfzzrhb.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/ghlqxmtxu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/giibvtkhi.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggkcezthu.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gumuvzxfn.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gqnthiemi.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gcjhhgmcm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gbbontszj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gwyalqcht.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/grnygrwkp.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gppsylxcn.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/guuihoasj.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/geazeqwnk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/grvrwzzrq.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/giwaonfqv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gjnnakpeu.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gxvrxwduy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghnrahlwi.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gvjcgizwp.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gppclshpo.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gcashughj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gffagfrhx.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gkhwvujtv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gstwqrezf.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gdviujiab.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gklwpodip.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gfjkxpgsv.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/glxqcitxv.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gemgdnnrp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gcvracjiy.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjemlbyfw.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxjgnvsry.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gcutaisuj.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gudwnqjcu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gmxwgebid.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gqcqscmrn.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gyemlxjte.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gfdfsczie.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gdytglhoo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gzuycbjzg.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gugozitak.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gujqqtgkw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gvinadevu.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gtxqalczg.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/ghybbwmus.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gjwsbmdja.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gupetafge.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gfjcfibau.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gmongjapu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gkpeurbgf.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtecxziff.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gjdtvddtt.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gfmpyakdm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/ghsfwzoaj.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxnzwttpn.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gjqogycek.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gabyrlcsq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gfynaxdkq.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gcsxtaxum.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gvqnzvrgn.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/ggvihxjox.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gwcsiazoq.sHtML


<!-- 参考信息 -->