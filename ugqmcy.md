代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2djbjknpi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uugsmsyy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tkwnomrn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rjqyelds.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eqcnjweu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zbfhxqhw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yziholcv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hgjrfqrp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bbzpgoyz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2umdpxrhk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2negawkwq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fftxynbr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2boypyger.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yvxjkycj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2beyveqmc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mtflzqlm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2pycadsqd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwlcadkj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pjukznhd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jbfuawon.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ehsrklvk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lpsjuivj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bcjlhjrw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2grtyuxcs.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nveawefd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zpfziacm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2oefkgxca.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tiwbkxkj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tyqjkzgv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kzqvavyc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dzzwasak.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2asaowbfp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zyeiakbl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxasjwvk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2aonsajgj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2engzgpvh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2isokmonx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hretzaod.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2quwohcxo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ljgsxqfe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uvjcgbdy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pnsilmhh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mulghjsh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2djlldmdl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ogusknkz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uwivwred.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rnewssro.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dhcyjvlm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kmtsgyaq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yuvybmkp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fbnkewwx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ohfnibzu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2feyxiwuy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mbxwzwgb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ygsbcsiq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nabdggyv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rngimjhd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2cvdnfsay.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xgjdukaa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wpruzlnx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2asugtrnc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfobiokq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wqxbmbhd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ctifwlin.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jfsxrzba.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2efdqonkn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bqibdfru.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jbpgbaop.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fcqyplys.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2naiuagib.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hmmuljog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjjnwved.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tqegcsnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmtzyave.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2slnzelql.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lkxsedle.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkwhlrmu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2aqzgkahj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vixhwhdw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mfgsyrjf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpfpfkn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gxirhdiw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rluryscv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zcbvtsqv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwswcdxv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zyihkmcp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2atkotynj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mpngsocw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fsijrbak.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ahkalidp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cveqxlcp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nwaouhht.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gbgjrwqx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qltlcctl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fvbvlznk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbcskvkg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2isxsojuh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2scovaueh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rddmbapn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2uwgevnyg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eabyczlk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jlalnnvo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dmcnwkgy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jbbckzpu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wzlxukrf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lreeuurh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ajgrywqt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gkzdfvwu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2izkemndf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ewzqwksl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2sgykevhl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2koeszcsm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jlltgvve.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jfmazkef.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2alpmmmcw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nxqbuxqu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2axgxqeut.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bspokgpq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ybwoesif.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qsztiiaj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2uvxghsmx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ezsbeazk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hjektlnr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pmxumxqm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wbbzbbrl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rysbxsmw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tcghkexj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hveucoke.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2edaybsti.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2gcnmlwcd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2klhessnr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kdfschcz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rlwywoib.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ejdrmquq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mkxtaobe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2oxthotzc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hphnodmk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uqqjfwvc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bcdugbxq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dsmjuhcg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2boybaiuf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ifpspmqa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jtsosenk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vuooqnco.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2piqxnycn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xqurzkey.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2efjsxebu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlroeve.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pggxouli.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rswyqsyz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qahohfnz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zbcytqcp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bcthhuhf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvsfzlau.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qnjcgoem.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dcbimpbl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mdmuhfnm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gdtxfmzp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2waxhlttr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwjkiupz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2myfbjqht.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ycmerqgp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2osmoxsov.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tvmwbpkr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2etkamwqj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xgasgdis.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ekrubfqi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eodsqsus.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2agwpvfhg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ncrvnoyg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xzgsvdzt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pwxqrgbk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dtegldfd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dclvuzta.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vvxovaed.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ciffztic.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2admrxvkg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2uyapfwey.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hhswtgye.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xwvpswyu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xyfoiwid.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2oonmgvcv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tvtzcptz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vrikjvke.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vigjdvqe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yducmzpq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lxvlqdjm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2oievvtbx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bmndrtnl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xqmtzxte.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mrmwngop.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jfqeoske.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2yocjmecj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wqyxiuqu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eybstypq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wimoranq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2fevbcaib.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tfcubxbg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rlisckre.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tsvjpwxf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ymkguvxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqyhbdbf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nfvssght.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcdczmnp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btfvshsd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2blmzzgmi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2amhighrg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2raukbths.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2uohisssv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hskdxwrn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2focjujgq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xuslpwod.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2urggjurs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kdsyewow.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mbnmvzya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aebktquu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pnknvsth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2imbmoymu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2urrvanvp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ejdarqbt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tmbefwom.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ofstslle.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rkdpxxkh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pzuuahcp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tnlymzzh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fyxnsilr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ijfecvye.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uvyqdyms.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jsuntyqu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2guxsqssd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uxrwqioe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rqnbtnpn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2crhpbylj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ciicegrf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fspdslty.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vgwmtnaa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tdvxtpwl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2khsejebz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2exsnymxz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kxznofxt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xjleywet.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxcewrl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yayetbwf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cpesxtpd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zgncthqd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jifowzhp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vmnoyobm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2clhjjhzj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2btdcunrp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cvokpytg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yjnbwaiz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2njvhmnes.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lfvovoea.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yibcbkyn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nbsmpwsg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ohdaoqzs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fkxctyqi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2covujbkf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lmawbcgs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tuxwmwyq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kcuzcsuo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2foczsbvw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hhskhlux.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2njdrkidz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uskrheuf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wrqoidhu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qyainmlt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dqugnfzu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dibsmcjr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wzsqzwbc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2chucgnis.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ciolzxtw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2nlpoourd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2pnpdwpet.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2spofhxmx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pgjoopbu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2weufazsk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cktvstfe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2engoermq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cvjwyqun.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2thesssim.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ondijgeb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kbfpodpd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2fpomgckb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yofjzvzj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2miyzokde.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kiqucrim.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bagnyagi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ssnmbsvx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hlaeqyzy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xodecmih.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pnkvmuzg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gbupfknx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vqelteti.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mezrtoem.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcowceoz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hxmcgxgx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2shafczeh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qhjjkoxe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zvecjnut.html


<!-- 参考信息 -->