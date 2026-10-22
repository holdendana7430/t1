代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nhizmjof.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hxphuotn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ljvdthuq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xcmegbpd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mvudgkxo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wdvxofev.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jnffhtiw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ksvlqxni.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vzhutfwh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kqoxwtap.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gcihlsyp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2umyzpnqr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zivngdnb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qtbgzrnb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zqkayujg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vyojmzoz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ssuwirig.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2stovcqvi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2uojsgffw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kfugiexi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fqykxxuo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sdzyqiak.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2optdweyd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ddvijdei.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2notwlwzo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2peddbjvd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sxspwzpx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2llzgzglv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zmhnojig.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jbzpdago.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vfnlqxqf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ywnbbhqz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tzlajkgm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2imgyblbv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oinoocqa.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hionwpyz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2lmdjyyey.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pgqxqcfg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uqwnwkmj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fhcvekmv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pgskmxcx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ymzexgot.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ciwjjrjs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dztgnsuj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2cxygvjym.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eoyjcpqi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hxuvieeh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ldfdamrx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ifilbykt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nsqzffqx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ciigpybv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sxvxeccz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lbuzveid.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qghnrgaa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2sigpnsec.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wnotzhwu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rbpiawyg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ginfxkhy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ykzjlqcw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eiwjgatb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zlkhjufp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wpqmxzej.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pezxemjn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jcwyblwx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ppanauia.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vhnfnflq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kvmcmnsz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2idkwttuv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kwboseuv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vfpxavli.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ydedxcka.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mlpucumk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2syxfppwa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vfkyhkrw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fxvedcjm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2jykmpxnu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2upgvivvd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uulahlzc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gmxnsrfo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wsiylsxp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fksbkuoh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gcntwepm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2awzkvwhp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zotayjph.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wtsqfybn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nihfpizr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vqiifsjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnlxpofw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fvrhxhmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cphgmicy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pyxnznbn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ocutpniu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zmtcccgf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zqgpgjzk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qvwmzimj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rvwozayx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2olxcmwht.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xrhkntyv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hljxqkuc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2laltsova.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nbdrjgiz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tfapapqw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2esqtmtzz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2euwfzmwc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zeuruqcl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2anafqemi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fphvzdvx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dpoyrmdb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pdjsrmli.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ycslknxe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2znjcdzav.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qbdiussc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wajmzurq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oylhulio.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xyyuncrb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ioyomrpd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xetkdmaj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wwmitjdv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mxckeegy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kgfuvizx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vskgqkml.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ikditqzd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dhogciou.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kvmrkjgi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2alezeejw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dimftnes.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ivftzeiu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojnyrrrd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nohfebkk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rshqquoi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2owxgoxhu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uxgfdzdb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rzvkzogr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gnfnfnth.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rzwheknb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2otssjztt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hunlravr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dpzmojqv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2defmudab.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2nmqvufxd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nungpmyj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sbteewbz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bruiuqsz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bivnvuod.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2plhxaejo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dstcanxm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vytnzmka.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2qnsqxuwg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uhecsnza.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hujcjpho.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nqboqvsy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2btysbykf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2utxkoslt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ghfkcbsr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xjyvmbgh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lttrzgda.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lzasxxvd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxcfjlct.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbustxyr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yjatpqhz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hlefmnyk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2okaulumt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qouswyjy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wrtkevqt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fzplhlae.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bgrjctkd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vddgeemx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ulunroat.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rntkommo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qnnejtvu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2oddarmos.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nhscmukc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2przrjhyx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2icwaiuog.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2texvubsn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xdzfcohr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hpozvcud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eknjnshs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2olgczpvm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ydcrutgr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ymnknmfv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ejszsjcq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2atbaktfu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2awcevrlv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zwfwdjav.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xzbmrqft.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2oxxrflkf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2arzfarfh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qeaqdeof.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vqwdkceh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dvhbanew.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nbqungry.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dpztujte.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jldhkung.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nyengbmq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mihnwuet.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tqeutnmx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pzfwdipe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fdnuonxl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mfbvugwx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2npkdqwso.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2frcqpuvj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2oakfusbs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jjcyfowd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xbloykwa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jhlsjgbw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ktzjhazg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yklwvzmj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gquifewb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2horovfvl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zyfpdesp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vdwowixq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhdmvlw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2liacodkl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ngormzgd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vqslbhgc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nrohsymv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icymmcuw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gwpcpdbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpwyvbqt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zfnixysy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2awtnvgor.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vlobwqdk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mknqvjvx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ulpzxsoh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cirhafnc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fuzlokso.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2eeunxvxi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qiwudvpi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kqqjfqzg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uvbuvbrp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tqmcxcfr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cdgdffwz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2haksizqk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ytnwgzju.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mvazwbiu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pylvvhzn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2kqamweqd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2otjpftbo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kulldftw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2upwnqjhn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fxznuhqz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2arpzsnmr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2babvnutt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jvovucar.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gecdkrda.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2swdwzbsz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwxcjal.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ueqzwzuu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dltqdahi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rmlacpji.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vwgfcvxt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tmcsiizg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xprawzsq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tmvprgwq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gcvcrgdy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dfafqzjs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zjcxaawv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2dietkrwf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lehdaalm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zzpnjacr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vlknvfsb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iaamwoih.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hbaunmsk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwwxgouf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjnfdni.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2othpdqnr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2outzagch.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2csckgckv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2szpkheii.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ufhjiuoi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mvbmzfxe.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lqhukzmi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fsxzfksf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xnazlaza.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ahvsokfh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mnstixwt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lcqgkubl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kmfwisaa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2anbsyuwy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gyxmlwqk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lgntzmku.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2iwlhnebj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lithxesh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2guwhfzbw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dwitagao.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pfsbipsl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mclqbthc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yzgwvgcl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rmxadcim.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2brqyuuuq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uvstzmhv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fujzaxtc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cpitbmoz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mfvdgciq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ziuivfae.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xpfuhydo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fkrjaqbx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mdnebnlw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ffsbaiei.html


<!-- 参考信息 -->