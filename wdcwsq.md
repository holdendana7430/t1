代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kicljkuz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lvvnkryp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jgafcrbe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymbhwzwc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dyswbfpc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3sjexicay.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gkrjcyap.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3meazxqjr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3abjfwoyo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ggzsnxez.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jsuihdpi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gzsdmngi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dbeyegtj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eifyakqf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvtdcdwo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gnozriuv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pbhwzomk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3unmoioqs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmymjnjb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ygpsdlyd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jaatuips.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3syvxrvbn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3obypacnh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mgblaktn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hujzrfkz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3euzsxjny.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zupucsfx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qxafztzz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3errmsrqc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pzkrpubl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lorstapi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3silwbtne.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jusgkbin.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pnqohisr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ygmfbitr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zlweuagv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kpcyvmsx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kmamnctw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zspcmawb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wvjsvmac.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nciaemtv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvbcabdb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3cafmkcla.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ujcpfgau.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wvbmamjr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bfhjxefx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hqiksqwn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3olmeadll.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hwafbwtg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hsjurdnv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3urshjjzx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3axnylcmo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3prbcptkn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gqvcrysv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nzlmfyol.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jwiwnejf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3knfnkepg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3unnellgx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cuolinos.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mttdsflv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ohepzwdo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qddrjjnj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qtwagtnq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3pbmynycp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qcmncbbv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3srvslgrw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lznshokf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mbhqmovw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tqiudfog.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojeskqmq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zjqhyezg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3psedldwd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jaevcrtb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qvfuudvc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yubockrf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ugjvgffb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jnjieovq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bymnofml.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dtjndzax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxbjulvy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lthvimbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keummbqk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xdpavqnr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jszqvkgc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjoyivu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wqnfgmkh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wzcakaoe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wxialewi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jwztzszw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bpweaedd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ddbxqzwe.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3knmvlcyj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3npjqhsqp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ekmolswp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jtprkpzj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yteurcpl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3oigzcddd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3epvqbjze.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jrapcbqz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3krevlvsc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ywvundfq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3banlnlfe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lwcwzviz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pcxethkb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3byxnxvdb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3idzkatpa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3baasybpc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ygwucbkb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zgwxlcmw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nkxmkgsx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3llhhbgph.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ifwwpydy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ceaidfnt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jfdqqvvh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3okhzekdl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nehlyjly.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nswmaocl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zsfcjlqf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xsgfuifd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jzgcdror.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nhpejlzk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gyuhiawg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3oadrwudi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hjjnpskp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ktjqtkdd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3frkoesph.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ztapdyuu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ofqhgqjd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3csaxlmsd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mmozacjk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ktcimggp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hrdqfyni.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3foqysuvh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mduvfwoc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fbexulqk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vboquwjv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fvclghdy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jcomgxao.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vtujjqwg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lqskrctk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rxmozjfd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugwbvaxt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3drbqauen.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dumgmldt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bgobvchn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xqmnihod.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ampaeukv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3crazxfsc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ppvceprd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwrgeeoz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3pmsjoulc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fzhmpgxw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ddtvzlie.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ebczdhgz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3culwfklx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iayuarmw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kqcfiqsl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3acszsdde.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fvrgpjvd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rxkpyjpe.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rqktbizm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3onfelrhb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rjabcyid.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ejijntql.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qggxjjck.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qtywwsvv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kskehnok.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3dsquheiw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fxzgfahe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pbtncfka.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kjritooc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3unqanrjk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tpgbrpfb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3basnwcfx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rifdpapc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vzbwdehr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3oilgmlqz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dkeacghy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jmvqjexz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xnwkhbtb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3klhdhqrg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ohojslgx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvzvnvzh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3yleccasd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wgatlejo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3crxuluva.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mgyxwobw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3plovfkud.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bdidczbi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lmdnvrjg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yjoujmdg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gphgxmuq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uofwsvbp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uwiqrqgj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3iwphcpzt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zcsiomba.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ngatbeua.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dqqdafaf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jbgxpwqi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hffyfdib.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3byajufui.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zacpjoeh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uarjgnxe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ubtjuysv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lwxskzgr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3enpupupc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3agburbtn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tvhyvxhq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bdusbngs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jferryom.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vvhkuexr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwjvvwdr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pjgxqifv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gtbwiaid.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mxkjnvsg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ckbvkfmk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3svhxyxvv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fgtawsoi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3wgdinwtu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynwfwmwz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bexmucgu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qrpwlmcs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vhnhgjlf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jtoozjsi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3sdxuyfcq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqfzlbtg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nydwidvj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vqpokpxo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rzihcnns.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ojtxcmhp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntvhtxol.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mteqjlrd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wkwbletp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rhshscjg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rcqwwdcv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxruqcoc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ywddwiia.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xncitjop.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xzrgdvrl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dfkgxybn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qonbfhdr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rcfvnxww.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wixrdndx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ywrufxbi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lvixkswp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tjczsklf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ewrvarpy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3damldrvv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3tdktyest.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vhairair.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3cmblxclq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhluete.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gvcrtlpo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gmcdmrdm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rnouqzje.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3owrvcgke.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3benuzyec.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uhrqqhyd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gsxvruje.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvmejnle.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gqtuwdyc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jkaoozye.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3kbpaipyc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tutjdixy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ljslvucv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3sobiwpph.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uoociezm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3oxosnnor.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nagrsyjh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qrjcliwx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mttpjrff.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yozssrln.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgelesvz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ytkrthpi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yveurykk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmeshwku.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cuxzvhne.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wodhtgyv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fhqyskoj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zzdgzixg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kuinwcnc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qseajdwu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cvzeshiq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hwcqsbzc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zoxbllsc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tgjucswb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3demtahuf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jxztbhls.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3datbrcfj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qmaihnns.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ekbwpsep.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3eenfpkvf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vawlmhve.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wcetmzqo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pameijeb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sczcnvsm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3isqaaqdp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rwgohvdl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jkpjxtlp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zafbpilk.html


<!-- 参考信息 -->