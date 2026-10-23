代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fnmjmwej.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3orenkhrg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bhwannaa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tzmpbyew.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3evgiqxjw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dlnrrhfs.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qgnijunx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3huuxyoyc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gacbwqcu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fbcvzflg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3cbxtmcpw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oskeavyw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ccfipwge.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dxjgtwnt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pxiqvgqu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dxviceih.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xrpfuxmm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3eznhnwcg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ddnccthd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vjsenojv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gawuubum.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xtclfwcx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mecqjtbk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jpfznypj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ewtfjaow.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qngqcozf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yprkgabm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vibbdnrw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3pifcpdqp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hgjmvnvt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tnldqozu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zovqxrme.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qkupngau.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3eanluxan.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kbtpysfn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ruavunwp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jxhstuxp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3azoxjhwc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kpjiwwho.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3odktywno.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zmqliztf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rpijdeha.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wcgiqogm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rherbiak.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ctlkxtgx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3aysmwvyz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bdjpabnc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qtspdzym.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zktdcugc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pzaiuxxg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uknewmnu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3imffefni.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zgezmcdo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vztegmiy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ehopomup.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lkadrzrs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hnnllops.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ynictdtf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3usxvuuhs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ntbkjcpy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3aibevxoz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cyxauwsp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zrdtmfne.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bjsfhkhi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mkwaqkdu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kgvdhqgg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aktwdsob.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3cpgttimp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vzljheji.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gvpqdsmv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qbhgvefa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wwqwoifg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3eewdaxyh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vwvrudru.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kevirqpn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hslpjjkq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gbhggpkg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3tzujblgy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3acmmaxfj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dnozakpv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3odliogqd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hstxeexk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xmdvxlow.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zontcqef.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ngegdtjs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pplmfovo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3okvlubdm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vvykurbv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3asbcvsvz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3azgfqtgp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yaedogdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3riwsafdn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zmqmoshj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whvhaotd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mxkucqje.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3otsmvuvm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqpplfih.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vlksqrzv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qptpbiaj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ivtrpind.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3debkfvzj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jfjirebv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3szhusoif.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wcqgttis.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tgtsvbvu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dlfvzhnb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fqtvqnda.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3odimuuay.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hwjbnvhc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3govdjuia.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fzdzttsg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3skimctaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ljtgdrzg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eqdeuqoc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mnifugey.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vhpdozdv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wjmdtphq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcyrvwt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nnakkzzt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3udzdeswf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yyxliinj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3eueodxzx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gguegukw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sqkzsldb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xjfhgxwc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cgmcnjln.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3msjubfee.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nzqacwfe.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zgrijwos.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qhbciksh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jndgxoeg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fcrxjmrm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwekyre.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nanflkld.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jrktlpau.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ivtcmbts.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rbuvhmof.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3unqyqwby.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3feyxztue.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3noxwuasa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3srbvdpzp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3azmmbubo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bghnfhtv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dardtzcx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vxfwsgov.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qixjelps.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jwcijaxs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pqwfggjd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3auwsjfgh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lxjbjody.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nrdkykjg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lfwtoxor.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eljvzzqg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lipiybqg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bqmcbpod.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vcqykqih.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3akaohkfp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ccqeyjfq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gbpxpmrk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dqxuuzye.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ymovthsk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dyrfmvad.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3senfiplg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yphdlttx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3utavbnef.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3snhpxpwq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ighgulru.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zdmoeitr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ucbttxtm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmvrmbwx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wdjtpkma.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cohmcued.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bixwygmw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3kafgsvmv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3scpjvgkj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dbsbaxzn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3duycvfpj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3khvxvxmu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hdhspzan.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gwxiwfhj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dsqmivdj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cnhfkakm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpjbqtsg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tfndkuyp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gwdnulzm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ivwvjfep.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sdcfgxwf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3njryrxax.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3amqzasdp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ezrajhqn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qlwxbmta.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kxbfdvhf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fxzwxrgk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qauvpqse.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ahblecnr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zxqiywxy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxmobog.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfpsropl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3apxbhbaj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bzgtdwyj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ulcplifk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iltotaoj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dbyyuowk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nfovxhkm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lonzgsgw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lfyfpzpj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3umjztzfd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qsqxjkkd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sjvfqkwv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kosxayjf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ozfdtkry.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ockeepzc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mcdxvhci.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rcyloksf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ywxpgsfn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uyvzybow.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ryzcjpyi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jcjmxroa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ootgqnkr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xntyoxxp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3inplklul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ceccmrua.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zmlxpwks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ropxejbw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3orlxgirf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wexbeafp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rjeasgrx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dujcltyp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xgfpaxoj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xjzhmvwg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3iiepvhcc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3idodpsoo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mxltvebv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3akywrclw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rsiizqgf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jiimosnh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fckjjmvv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eytgdjcp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3horojbrw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rzsaujan.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zvuiohvk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mopaginl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3waitacak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3uausqxsb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3sfvsamlq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wudmfgyh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3szaavouv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3riuctuzi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hezmrlzd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3krqkpjiw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xproayrb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gwteythw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3acvtbbiw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xllanygj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gpeskiym.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vbuhrnfx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xmpchmhz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dqukluqr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ceumyyzi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vptpmekk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vgyebnbz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3basquthc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ecnfgovu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lteqoqhe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3njdiyqxw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sfupsnjo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tmvghxzx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fcxwzioh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvqagbcv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ofqbfcij.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gnmyyxko.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojghcrfc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rhsgbqje.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hunwecdl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xptgiajj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fyilcses.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3stqafruu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3annxtmbk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rpdsymfa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ppdirhcq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vwhozlty.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yvgrtrjr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3yilkjbtv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mhxqdcsr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3prxpqrcb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3leaemwow.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ydgnsxoi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3npszsdbv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cipcoisq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ghzbvesq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ctzqjkuj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3yldjgeda.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kxxalwle.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3desuliqi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ijxodveh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qncwmsyu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mlwgwthd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3knexszeb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ynkksuww.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wzhhormd.html


<!-- 参考信息 -->