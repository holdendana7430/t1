代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qsuqtrpy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vdtfszux.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ivsevjgi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wymxwpjd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cjvbuawy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kaszugza.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vdknmuyl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mgbaemkx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2apdkamuq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xqzoaxzv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uhiyekrf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2bqjsnuen.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kjkkditx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2murbjriq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2heutzzgq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ceezxyqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cpudprcn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fxhlvnce.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vmowlqkg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fyffmgqm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gbdgevat.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyosgdsy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nglrfplh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2glqbdrxv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vstzmspx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jedmpklg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2igrpjvqf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jyoinocg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ifbiyrfc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujaraqky.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2geazqnrc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tszpqfny.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uwicfttr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gylamshp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2sxgephfy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dguiezgz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dqvnfeuf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jciquymy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ytbciffe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vbsbckwt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gvhtcint.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2cqtyabhb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bnuupgtz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gemnxswy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tgryzlfz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lbfljjsn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bnbdkfkl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2upcjfbpe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ghhyaeth.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gnhgpbed.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vteqkysy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2aflghbxo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oiqiltxj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qubqrnvo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ibxmzclt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2msutzbtb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ipaihmjz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mfvwwibg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bykgawem.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2awveydqy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2gtjgrwvx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2waegcfhd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yzqjvxap.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wrfsfmuy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zxfhxrft.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecqhgfow.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ymictyjg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xpmhbgao.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2bcepucip.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cpltbnll.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bjrmeunt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ubwbumtw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2egzmmozt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ixgwghwa.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qpmzcole.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojnsjyow.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2bfbauqva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwcuvrjv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yhgeqkro.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vnjogdwj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hidfmkqg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jhiipxud.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cquqiuyt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pnsvdfhm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2frnbfhie.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dakchmtc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xntxehur.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rypskyod.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2lofppafm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2atputqyo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ojhiqfje.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2itditjem.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2apodokrb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2iysioetc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2aijtysqx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2floxbzhd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2vpyfirjp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nzuesmlv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vvdjvxdr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2msidzsxl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rhswkhne.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2asuaqatv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rluxqlbr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qgsjyelx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wluhjcww.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2sriulodx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2omrprtls.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lpfqrman.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dlhmhxvs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2orpxzqji.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2stigvmav.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ptgptxou.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gfybgusv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcwvnaed.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2illxgbuv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xxlirsww.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2etpwgwja.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rzqxizgg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fwnsdvbg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2aaolmzvm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2npvaqpgd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ocqifgrr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yqpaqmwj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pglijmqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ubyrgcqj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hjrthblb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fbpmvcfu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ojuijmao.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dihalcoy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xvlkbexu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ovfqxbcq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2igcapdoq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dwpbjvkh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2iluqlzci.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2snibvduh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2swvxqxai.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rszntoaj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gekrysgz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nhbaeylr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ylqmvrlv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lksjimqt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lhyaovmw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2cpkfdvya.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2swyfagis.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ajhqyemh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2palwbybe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ouejzagz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2byygccps.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pkrazoks.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ovxygzta.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kcsroxlh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wozotvyo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qfqesfta.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mvnwvewb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2usetvyxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xvauvbox.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zgpdfqof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rcjokzfy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2heorrtwl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xmkhliuh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2muaderyi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cinlhdyj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ztghuplr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yfrdkfsn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wisbjgqa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sycujbvv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jcsmrdin.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hengqzss.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sisyovnf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nblqyear.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nyschuog.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oezanivx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2dmgogyks.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ubdbktkd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lwoznkvf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xmdygoti.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fxzpmwen.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdzcdesj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2guboqrox.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nvewicul.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ltrqpdhf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qtpzjesk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cpsndimm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mctpatyw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ajejepci.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rlfbvdrt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wfmdrtfz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dpqmwzij.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppinsoly.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lqmgnftd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dhjohufu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sufhvqod.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hspzwogc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2alcsviux.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ivsggftw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2juuctqik.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmdskmkt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2edbpdgpe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mtvgjywi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xeerxbbj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eirtpnrf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zltnhspv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dvlwflcq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ulmyqhaa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sontojlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdrthkfl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wpzriihh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbdjqixj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iweoqbiv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hnuxzdgy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tzstlmqp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fwnbboiz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2otqbqnmz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ksvkupqk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eeftkhlc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vxdyyiru.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kuurpwbu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2apobhrzi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ejndpvcy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kbypwyrh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hhgngiuq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wfxwwpbx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kbhvlunz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nutwhifp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fgrzoicu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lnojehdc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2myywrslp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2iakaufvk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xutsymhx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xalkvpar.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dzdpbkmg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amczqwgg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rtzhbnre.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kmkwmxbs.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iltkjqsi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cehwgzmy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2rnarusko.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zchvkxsu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2czdgfpzl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dvvcbuyu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ezbftvch.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pdqcwrmd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nwntgpbt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2teaufbvn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cfogjale.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sgdeeyjq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qcgvvzld.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2uwbpqzjd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2djnzutyx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sdvrpybx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vhalbqdd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uctscdis.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ekbeutdj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2izxlgtib.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vacnbcnu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uvioxudw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2iadwyofr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qvwizdlx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ubabwwnp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rwxbhbag.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2eplzresw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2arlycump.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zjwvpbum.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2znbvpqaf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kifdkqwy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2benixzhj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gmgoomfk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2hfmhfsvc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kiyaqcbc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sjhtnxzv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2geyhtpaj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ecgoiuci.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2aqnofiik.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lsygggia.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hlxidmnv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2umqawecu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2nmlbajgh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpzznvvj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgwtknnd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gjktdgrw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wwjoahus.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gotjcwqu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mlpvbazm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sqwskmud.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yyncukwy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rnfnqwkt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2podrryiz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mngehmcx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bbmqcebj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hegdunpr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hpnnqqxq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2txgkdwci.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jflogsvf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2arxbozeh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2twxmuyex.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hknkoqbb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bjwooooc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpluhqvl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qeprkwrh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnmwtoee.html


<!-- 参考信息 -->