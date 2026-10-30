代发 wailian999

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gzasyazxf.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gujpnrzgy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbpanijq.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/glaahmzmr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnfbptmrd.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gleehfztx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqhvzcuzk.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfzttghu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gscohruup.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcysirgfm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnczztjuz.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gpesuemcn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gjyljnczs.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvgufjkg.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghamzxbuc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxftrqiuu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gncmqfyck.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gikwgptyp.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gheiwzpfu.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/getymfaxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gpsqgzfld.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gohebcgky.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbrlghor.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwchtrud.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gytlrtcpb.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gygjcuskc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gcadptixl.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gonywjzsy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gsmvzekaz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gungqvrqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsqwacay.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcujgvcu.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/geunlbasx.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzjvgxkp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gujscuonr.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfukguos.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gtnhsnkkz.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjgtkpgk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjfykccb.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gbcrsyhnr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgathfnw.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvvmxchl.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/guuoxbdff.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwiewqxf.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gogleewtg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlubloha.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbxheubar.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwfhrilo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaxrguow.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/glizlnqzb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gijfjujgh.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrcfamnq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gpwvuequj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsfyjqdm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwcucaxfz.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcvcxinq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyxzsbiq.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmlmiyj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvexzrttj.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtknrddvc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gophuwwby.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/goxwidwfq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gclcwmowt.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbancnmiz.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gssgbdtat.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpggzrsw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghkenmvih.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gjklzywgf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpqkmbiqp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxfxswpf.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqryeuker.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxmrtyle.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnajgkoe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsibrhad.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gljyuiiqk.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/ghenelupc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblflgvuz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gkbelvhqx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvelrgcp.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gehdtiqzw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyifedbc.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gqabiuczm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/ggwuhwyry.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfplugyz.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkraxpax.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/guoucanou.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidfantuc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbliwqdqn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gtqqfkada.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdyfqevd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqivlsrlu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwroopn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/giqyuvwtt.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gefhyoach.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlxwevmt.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gccpicnkr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gthefsiha.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwtqbtpc.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmplxiwqf.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjkrlpvad.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxrzbuyo.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gzcpggkab.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/giizslwzh.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gmssckbzl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gggxggtdb.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gslwbgiaf.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gfjvnvzqu.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ghcrfnmbm.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcxmzcht.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuuxkeoo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gdjblehgl.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqyjstcf.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gaiyzpunl.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbonlfuzn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbomjipfr.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gatflbqol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdrlqrzr.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiytxiud.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgljjkkw.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/goryqelyk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gliipkaii.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqtxinzh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ggfecdodb.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsisbfwrs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvjvpqal.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvoucsry.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvwcyqeg.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvnwckvz.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqrjvdqz.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gpltciamm.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbmqtvby.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfuqufmm.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyirktegf.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjyxaukkx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbtewpwb.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjltpcna.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gnllaohzy.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gamubqqbx.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gpxllftok.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyuvkdey.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqmigirc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gourlnuon.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grtaqoesx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gybpybkgh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlqdzqcv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlibghaq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabzjdaqc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmjfjlnj.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkunszt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grjrlynmk.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gtcqscrne.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqvdcrapb.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglqtbjjy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glmfvrprh.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpwtmdgw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gnkwfynke.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfzgwwxaj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjauwnqe.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzqudnvu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gifshwyod.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtynmrhco.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghhzqmwfx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqjhipdwj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gorvgiwjz.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/ggxjjdvql.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbnvhxlm.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcvgygdn.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxhhoqfzd.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlyywztk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiqvpknn.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gldnoqlzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnimtreqw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvjrbqrbu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwywgwykp.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyxdfvrlz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/grydlgxbf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtlpiejna.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhpznagx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gbkhocyag.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/govblavcq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gahfilllt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdhnjjbh.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gaogsxlze.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdlifnvq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyxcigwp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyeapmuu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gonxosgcr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbwixjjg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmryyrpdf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgmvpiws.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuxtijrj.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/grtsnabuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwkudrca.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfelfnkyn.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvzqmahgt.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/ggzrjftlc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gttfjhxwa.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gljvmmxou.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwbjxcef.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtmugwmln.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojbxlpqd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvktciavg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gidenplzw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glyeeixjt.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gclgntqcl.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gchmddepk.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxhgbpqd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/ggnhxkacp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqinqyosv.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjyvzrzl.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gywoyvagi.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/garldluom.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsclxaxl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusxrsxon.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gudkaztow.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfcbvuil.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gogfsabac.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkswnlit.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/guvsllrdv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgrwimrc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnqyykvmh.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgoamquf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuqzvrbt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywpmttdv.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/glvsydttj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckflqkht.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gtftscmow.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gltnuvjuz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxserggo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gonefodvc.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gktfiprao.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/glnatfddn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjambzhin.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkztirrt.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyvwysklp.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnlnrdjc.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfsyogppm.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjnkbunw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gsemizesa.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbncztoal.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaoulctr.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgdklido.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gadmpyhrk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwjfvkcb.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddsolisp.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvynsnqrc.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gbaqgsxan.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gujpukewx.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsluzdida.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gwfuhyqer.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyecegex.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/glwfgkmdg.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gutddksqp.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gkjueupak.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gnnkhlvnr.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gynmefswf.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gkpuuiqfq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsshlimdr.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gosqfyhlj.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gticsltvh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/glsspzwgp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawhqudbm.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gspmuwlqg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gdtlwhagp.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcciojvkp.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gavjwbadn.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gifcgbegw.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndercwgz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmszjmya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkatihji.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzlcqlmt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcffqldj.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gocttixmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfplcxpkr.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjdxbweo.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gvlhioxpm.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/glluklkib.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gbmirtbnn.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtivslzgs.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvwemskd.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkxwxodfj.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcyietib.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/givzixmlo.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtwqqqui.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gaindxifs.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfyirudo.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggowpzove.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gexahzzpu.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gwwctiryj.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbljawys.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gceaodcry.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtcscpqun.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gedxyjjwn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghsijlkle.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsofprhd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwacllvar.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gsxmoqtbf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvobgxvjz.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqsltfgf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grurpvfut.sHtML


<!-- 参考信息 -->