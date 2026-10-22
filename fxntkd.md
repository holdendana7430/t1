代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hxkxgqah.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2amyygxpr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nbvxmvfq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kxjumdxt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vdwhisdy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ovjaipsb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2limlkhuf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ulxsyzvy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ntcnlvxq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2oxhmibem.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zflhuiny.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vbuosxwc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bdghvrls.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2upyaelkf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yyjmmgnp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lzuknupr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2htwpuekl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2itazfgso.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2sifmdvag.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jvgmcxdn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pastejdx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lkuqbmlp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgsdcojq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lnmejemf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tubxvfok.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gbrmipld.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2paxbfaqu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2chdibkhb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qzifbmox.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xjihiurp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ihgstqig.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2djfjhpfz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2lcehjvnr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kxeewlor.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mjoxcjft.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rqrcydmt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ikabvryj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zjbzaiiv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yjcroyhq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mgbtwzbu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lpbyzior.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lfdqdfnp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lrstrmqk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xkjxzmcd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kscrzbiz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2krewbvae.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kosjyoxl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bnwvhvzq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lebfcums.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fwmnywtk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2lmdpznke.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xwttkphl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2sqracuzq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jrrgoqmo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnbwifm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sksnhtkz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jvszpkjq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qzdkykwp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bpyefwio.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hhxvzwjq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yemtobjv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ahmzqbzi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2avtqkydq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dqzktxxu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pszurbmb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vhhfvspc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2umpbazpp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lchcnebs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2efktcazl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2renzwobk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbnvscyl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dybwxrmw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2yvcamfen.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2oqqpipgf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ilmryfsk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2musytgpq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jsfdjyad.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rubbmets.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fuvmoewd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jsxvrjpu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wpiktdir.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jgxjxmgl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ojvaaumc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2igzsmuru.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bextuvrw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fzbfqruz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yvznotjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llieceru.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oskzamoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xezkkwat.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2angfxfyz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pymvnetv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tvdvheyk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ngemnved.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2oueqbntd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zrhxkvky.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qsgqtvso.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zeaavpkx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xchuyctn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fovtvnsk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kguareqm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ucjngiln.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iberiszp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nuzttqdp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rrgfsxxi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mvmuhkjt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lzkozors.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2szvlaavo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sufptmno.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mnqwwpzp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zrvqfbgb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rqgqqqto.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gvdyhuiu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iafsjfbu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xmswcnhy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbasnfka.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2atupgfiz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dbembcfr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wytyzadf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2skbopgcm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2skwxugum.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tevwduoh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2otgbzzmy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zpckkorm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jickaoen.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpzffnad.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kznbubmn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zpjokaza.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2uamjvvwq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ggqvbval.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bepbrbdl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2afyxpyqc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lfzeaxpo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2modumakj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rdqiaedj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qrbnnmkc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qgrvclfw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kvlqhtjy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bipvlzvw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xwpvrcdy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2epvqsgkc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2toqjvlfz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rjvymytw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yuubezia.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gzibvxvx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2acudvrjm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aqxbgiot.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2njgzgtoa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dbddeapi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbcfyegv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dsmajefw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rzygwlfa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tfqtpkvx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2idqtpdzm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ejiyhupd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ovtmcnbk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmalvi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbyxpsyb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gpnyjhni.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2daeydels.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wxkrxfos.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fjnwzwwc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gilypgcy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nrzninyo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mppdaqdt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ligusctb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tuadkdku.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kwrsuxbr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mpbpjbmw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvghzdsp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yjuilbzy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nctfdpof.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vxwuwydb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wqrilbyg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyecmfjg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tahsabvz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lnfsibfa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kjputigx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cfgixrfn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dxqufsec.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tlzxbbqt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vcdimcaq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ozaqekcp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcdxnnqj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gaogparj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lltkyaxb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nckecxpj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nrgktqsx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rssbcxee.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykiuuojj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjemqvob.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lwdcwtpy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bctduptq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mbtkoubu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qcoxmmwo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dlofiwrv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bclehluh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dtpltbyi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yruseyil.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cjfwsips.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rxogdynj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gpfpdrja.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yvcehlgh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nokchsrp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ubjckvhq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ovjuowtk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2odqvllpc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zrbhdtrc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qajzjekd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jiaykscd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2obujvbiq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qftixicx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zcncreen.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kyvpwysb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vvmvnqtz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kxahlmhj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hcecmsoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwewlsbx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nzweijeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btqvtzni.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgcsbdxz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fejxyrsa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nzjgzuzg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2erwojftf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dvzqpvwy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qtuitazj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cgjmnhnj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cwcvehew.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nkwbrzya.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tqfkyrbi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qxxvjrco.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2thepppbw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wamanaev.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vgfvikgq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ajcaufgs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qwihvlwp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ucxykykt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2sshqhekh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bspaudxm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ufxoxdrp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ygydcwjn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nttyvtsw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bambikgi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2akxicqmx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2oharnmjo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2huzlvtdn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nscjsdhj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hypylflj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ouaaznqt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2wffahhoc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hgkapnfr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fwfkvqmb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qlpnijac.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oachbemk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ndmkjrsl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xlosnkcw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oawcavki.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2uotduife.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ldxeltfr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wfkcxkkw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bkpdunam.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2coqtnzpm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gdecjhdi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2swebysyw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uefcdjaj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pfutvqyh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hfphyvue.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dcoxyvib.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2knrjiour.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ivtkranf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2okezmdfp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ltzkbxua.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2khuvhigw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sfbrjfrp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2quguqcjv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ddqjeqjh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fghicvcc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tiqqhuhb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2subixmaa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kbovlrto.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzyephdz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2shcomrqj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gdhawrln.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zelshmoe.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rhwutfyy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rubabgae.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2eruvrlpw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2egikqlug.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2zukktdir.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sffktmwy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxhsatsw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lvnrhnly.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fuvwdnjp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mvypvkuz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fsieztnr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gqkafbyf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kntrnuht.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hvtxqkki.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kooduuxd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hqcejgiz.html


<!-- 参考信息 -->