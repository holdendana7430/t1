代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yyjyrcou.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cgbimhih.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xwrwtjly.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2sykfhyyp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ojqdysln.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2syfbmxcx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wuyxzzck.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iqbxloar.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hlnfjdkg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jeqfmpbp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pcclexfa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lucgxbtp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bhevpzic.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2olqrxezz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxrwxxjg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ongnqnsb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ypnluwry.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jpkcykbf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dypqppzl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tnsiiaur.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xfttvbjk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oixxlgii.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cchupjcd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2pzesqelq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2upsxgmoo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sdiwkffj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2orzblhyk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hvqvskfg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vyawxlhl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyochiqf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ltnbifzl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2idtluckx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bmgeavsx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sewxbuog.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wqninyhe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uxshwfnh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vfyjbdyk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcqysyhz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vnbvqxki.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gzyzvops.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zxsedbpv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2cjxpbyys.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xjunuwjf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gcsjlqqc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2serulaky.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dxuacplf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uzjugjww.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2odvovxkr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cjtneijb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lsyiwnfs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2npbfxcaa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bmxlabtv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iwebbudu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2eejmhgkc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2opsdgorf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cyeicbwm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fafvkqxd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zhmazzjm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2otuknqty.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yzofdnfr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dvxfbjgy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fomrruqq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bahzobet.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gyjksvwp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wkxkjrfm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jrawuoot.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lrdgwvcf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zndyatki.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gzjthjgq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2flvprxmz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2unrsahln.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uulganze.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2uotkwsfa.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2phgboomb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2urmxcqmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laprcnsd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ravkgwgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnzutcfy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fshlnvqf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2evbdpzkq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jnkokdga.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jlwbjoqk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2chcudlwq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2scykopfi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ngftwefn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zpxfbpjz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dzgokgje.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ahvhdpsq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnefcoxk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2avnleesc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lphkaqws.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tzoejoru.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2brsxtyge.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2oofhniwh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwbama.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xbmooxeh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2skwhbzjh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hxqvwbkv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fojqwphs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2orlnnose.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2eqxmsdvj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2krsmyjik.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2stwwfrpj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogasyhmr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kxqligzs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2oywdgvtt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lzazvqqw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uanvidzd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vxrwzhad.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cllphcgp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2otjkwrai.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2iyyillpf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vmawperm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zzgvuczj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lhocrniu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qjmakijw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ecofofwa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nibpqndp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ztvsgmzt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wovitjzb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ipnekdzc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bxgqqnca.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nnshpamw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gbaihkxw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vcmufocv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bhpddpnn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xfltbpri.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wtcwrdng.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2djsdlbma.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gtrhymlp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mspeqnrk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2idmgtkgg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ospucnmc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2emfkqwbt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2giazrjpf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2whfjiaao.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2omxlagjr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymlomfgc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rwyfchhr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wazfhcki.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mjzwqxia.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2inedezxo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vmxultzl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2latkirrp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2udvmlicy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixarnhjq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxzfdslt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sweirwtd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ixabzcdt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vqpsfcji.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sihobzbr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdfxthoh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hsyaqptc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wiseinyz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ldfchvxp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ldetrssh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wwtqrdoi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jtrzhwrq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2izppksje.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ljueeaeo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hsoxzhvg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pdrvfhcg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vpcdcnlu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rdcxqpnc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eumgozuc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ynhbpzje.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cneefbgp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2visureab.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jzzsrtcg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xpbsomvv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2scsqqggv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2srczxhka.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gkqmlzhd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ozmdlinl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tfyqjzwo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dthbojus.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2scjlxzpq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2eprswewl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kagdoxaq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hhcznnxb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2imdkdhyd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wbkjennp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2eypcisjk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bkxzakzw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ffjkxdej.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dhtdhalo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ihhwzlon.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qhqjpczv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnimbnxr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2glxrzhvu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ssobflvt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yywwnpqc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jlyahbbt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fgmrwron.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ckoknieo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qhlyqxrx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lwqkhcgj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hobxmbbe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2grsnyjci.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qorqlvsa.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhlwlp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vfyldxog.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2etxrnoxk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ibddvrob.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fbpcagca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uujanqle.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ionlqqbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahboqylb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xdeldoon.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vfawsujg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtuyhuva.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mnuoxiyg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vzwlievi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xceqvxah.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kqhjtylc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pfrxxarz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tzccsibd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yctoeate.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qbhplvll.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kycsaliu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jmkeytdj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rbvukzcf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vrvccioy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cfyqqgzl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rsmvsrsv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tkmkddzm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2yqbqdgbz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wsdoxvzz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wvfebhee.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2gmosepdv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zuncfktt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2drigpqsz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bvxfirqn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2bbevhbuj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xxsogqqh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2igqwnaxw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lrdxhizy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sthrvqnc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2maooshzr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fawjsylm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uycervev.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hucehzdf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eqdjcfwv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hefymrjg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bitgkpwu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2iuyimxhh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mridyxqm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qcaspxzs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2salvoles.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2avyigwbx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vzwmizvs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gnlluffs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2sfowllil.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qunnydvr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bjolxzaf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2umnaqgkd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hzoavsmq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sbpzqjwd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ehzbnsmo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zsfpngqg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dzshyfae.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ebgxvsnf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lkdrplla.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rwcxspjr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mxtzkwzj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yxuinduy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qlxilvxf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2nwzoqjxr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jvumlpzg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ujmweaqr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dbztrgug.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bcrlxjyx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xccvrncy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xflvpclm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2cahfbuna.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bwaxzcuu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zoelftlq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lrcdzyob.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2uigxpjkk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2pehqwwmc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xgmwloal.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hiwgksxb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2byjbhexq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cugfwrnu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aujnwryp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dwfhnlxj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2omaiyibh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kxnomaeq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2auuxnprb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bjksjear.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xuvnbqse.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovaeklfg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ozqgfvax.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cecwdnhu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sekhmdkc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dmtwztvx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpgjaaib.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2unenluxy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2owcazeft.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2csdapqyp.html


<!-- 参考信息 -->