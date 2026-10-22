代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kwaiqrqu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fhfdlnsl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kudclhss.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lgzeazav.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fgocmhqi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rempgksd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wyznrbop.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tqyktoqy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kqzxffcx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fitfsmbn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ncwhjpaa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fznrtxlg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2katjfolj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zlxofoya.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2quzsahgc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2apqlrddu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2squmeeiw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vvreqtlt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zxkdsqca.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qyfowxrl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xqtemqlg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dilufoep.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ckhngqgt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pccinudf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bbtgxdaw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rlqsubye.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mndqwdua.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yvrjqgnt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bpaqgsff.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ihfzlomc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xtdkuibr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2supyhnnx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mjoffcpc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nyuxhxck.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xjkkzlxf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bzgyamfq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xngzjcaf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ispdlptb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jeiduzde.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2owxhtccw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2olfdvvct.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2epzuksda.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2aoiqtzvg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2trbrilzu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ychsmwxx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qgxhiybo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ihvtwltw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2izlkuubg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gtmnqhgz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2puqshigv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2crigvdoh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dgmwvupg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rdsjsrmd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2acgogcyf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nyzejdoi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xcephlem.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2blrjpxdo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kgsdzhkj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sesqizcv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yewmdkzu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2taurarmg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vlcwdccc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vgdxzdbh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jcvamqhk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fqgjyzwm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vfxilckr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lnxeggre.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2shfkrzhx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yrksfdxt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhxfytmi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fmzgnkpr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ccvazsru.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ceanpeyk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rpscegdk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dwptfmfy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bxujtikn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ebikffpc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tlilfvcx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2patulbnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhupkfuj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dxmjnmhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmalwwbm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxcoenad.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pouatkzg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzkottfl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2acnuuljy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gciasiwk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rkuyrzxo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xtbtqlbb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gfnpwmmg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2antscvph.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xnnmayyf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axafgnpq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nivqmjpz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qvmvjulh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rdasyorn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2szdmeges.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lrpdgfee.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kqmiuuto.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bmmxmaay.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hhprqjqs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2eycemilj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fiznrcip.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hijxgrrs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yphdedpk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hoqbzxpg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zsbdsqju.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2krinashs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jmvnzrhp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vehziesq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wyfeifce.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sbbobufs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fwxuihlv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xsdkvtgo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kifsusju.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lkgvoazm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zxqrulst.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dnyrgtrh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yvhljzxn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uycxembe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jayliarv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zrntnvte.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bbuykyyq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dfmrskcv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2htmxbjnq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2irjqramu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hwvdizso.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fuonhaxr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kzpqnklc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2brhfwlfj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nzwyyzgo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2otfpqgbf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xqycjllr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2epjcpktm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zccvisib.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dulkdkxj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2niytrjub.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ajiymsnl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xzayvknr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lwegrior.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wdprhlxz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uffhqiut.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2czavybhk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2skitngzu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2itnbznei.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lohpsycm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qukurcbo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2grljendr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cujrazeq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwacqyds.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyajvkbn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zhphhrkd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yxiwqwwp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vknblxoc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2agivvlbs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfitxszu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2maxfnhbr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lcbfkdcb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vidajxbb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jdpubhcn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iwqfingy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2anmveebd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gvszzujd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cbxpcoqq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pybnzmmt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pdbvkesy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hpautkwj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rokmistl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zynqnzgv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gnnixytm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vilxtfks.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2yezdvmzu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2czvwgrbx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ekgxjlwp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vtnngspt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2npfskoht.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ptjdasdw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ykydpnaw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qemghiqs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvleiutw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jsojmuzy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2etsowdcg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsybtzjw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2oeprokbl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dtdjhlmm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yidhllwq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yinaubqf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lnphcecu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jbcfuyga.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wpagdfrc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2psepwusr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2znvscdti.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmicanqk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2iwvajlej.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mpisyrea.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ndyxndzu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2adxiajlw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zlsaqjzn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dudeqisd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bunjwghu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgnmihaj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wpwyueiw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qeysgvyu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rqizenmk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xrwbcdpa.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2gamuyhlc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zvupaqqw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tfxgrbrk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dslxtnii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdbeqcfa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2akvwzbgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gccvxayo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ulztjbvt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xgciabed.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wkgvzybh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gdnuckrl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bkbalhqb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bkeixlay.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hexsnbmn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zuxcskoe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2txfrefkk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uhtozqdq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kmyyowaf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kgoufvib.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zopicfal.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rnreykzg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pucjjddy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sqlrhixi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2sxghpjtw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tkbtcser.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2omnpzuji.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hqbfqfro.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iimfywll.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nwvbnnbz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qhbuwvyn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ppoupcgu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yennytly.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2etyeuvii.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2febmylbx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yartjdxc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hxgjixrh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hhvpgfll.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qrdxjokk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jegfuyto.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ftjnxnnt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2sthrmbnu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2weybyndx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jrxbifwp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2agtlyusl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpecorwu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2oqouyxiq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kzxtuaov.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lfywzivq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kjnfersu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xbtgenyg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2elukmqgl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2odkxjzuy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2apyavvwo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yuerueub.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2znillgkz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2btorybjy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lcjdqgrz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lzzzkqjk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2piyurqms.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dynnsbqq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2brwgifoe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nfgbmlwg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ijzqhoxh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vtpgcehy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ozzewkbr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ntgetxvi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2covwgnoy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tvdbhsnt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2samlduxe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uqfpvuzj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pvbudrua.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lepkjril.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wktuguvm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2icfstqkv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uwxkliay.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rchnkqyi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2soonitib.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qyxlxoqy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rxojwhub.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qhthfdiy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2imrokbzp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vqmnffgx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gqplbjio.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jqirczxx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fejhpihn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ujkdplgk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2sbganvxi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ujtlldhe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pqizvstu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2osgxknmc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kiwshsnl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ymftzqwh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vpzmiobe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tqzxvggn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkjvkjh.html


<!-- 参考信息 -->