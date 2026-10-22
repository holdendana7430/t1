代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gudahjym.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2yjleqggs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qkvghmvv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jibkzjiz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsjwvgty.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2twleaxtm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gsorgxri.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ridhwecn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hubliccx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2efmzpxfc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rmogrrnd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2iffvkrgb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pavuvyli.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zxjnmivv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2esmvnfxg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2csdcmfpq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2shgjmhai.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rygtogbb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bdhczivr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bwrmhche.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ohqvcfxh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2acpinsws.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2brgmxfcw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gkdksxwj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iyshfnkk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zstuqeia.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xrozvjvw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrpqgecw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2eaowxqsh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kutwqjok.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fatdzzsf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2umnslyyg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ddbjtpyg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lsacgfet.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tpnwzzkt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kuekekjy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2cjtrmcpx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kteftizt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fetcnubc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ehxtyjpn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fwadkdsi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vlvejznx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ppjdrgpo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pakagjkp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dckextgm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2faxqrjen.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xgowhirj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rldwxxbj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2izljsslr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2klxdpsht.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2rddmshjg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2spplwsjx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ogfbkwdy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjjxlioq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rowauhun.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2olcyicpf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lwkozzho.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wbyujroh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qwmocbiv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vwdnetlu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2czsypjrj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tftkadhh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mevktpxd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jzylrehj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ofnqkcoq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qwjzqlif.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxoxcgaj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gqlczzsp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vqwggaqv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bxgcibca.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ujiyukcc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xarlbibv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xzjtqviu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2oyijnyse.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2delzanmb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zlfmxmuh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jvgvmdfx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bxqhcemk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sbrgbjid.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymexyxib.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2sueuldzl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dvjapoer.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nkqfpiig.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vwpbjscl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mmpkvdyo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jcdaxinz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zpzappfc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ubjfdmlg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hwfdyfpo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jjaxsgyz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rvesvbfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slfmddsf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2czsujqwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xglispuu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxxozzbi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2opwdnlpd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fliyyngc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yxywhjry.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hrpsmwmh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xmilggkx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qulcgjda.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nxmmgrca.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xiaukkvn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aqfuxuuv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qebhszwc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pjtdmjbl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xtlztsak.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lniktolq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qengbwit.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bhmeispv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ztozqakq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yzdxxtgy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gltbwwcv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2afgnymis.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2avgkpqkm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2olnjvaft.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vizsvndp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lzpjkrnp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nzlegjdl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lmbbtkyd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ermefrru.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2umbgpifa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qxpnrnyk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xiuxofak.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cbethrcr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2thdzjbjy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2daazkujf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2enwtjjzc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ogizyfcf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uiobbsvz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2phwnrmmc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dljsyely.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2puiojxyt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fqnshovo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dhqfehfj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dzuxjbtn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2agghjwtm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rdttgmbs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2wmsqseeo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2khahonrx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ynmzfjqy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ijzlvmdt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2uvkufhta.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qgusnpyi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xyzcmlpo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zseeehyk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hdxcpfnl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kfflslcf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hceoraui.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2povielfo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rbytsukv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2igugbxtp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xaiesmna.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwwcrilj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iuwdvceg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2htpvzgog.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kghyqqfu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oumpkrev.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2urzfogcy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2exeufmxd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nyoqhotx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ukldaylv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2diclsnfv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ecqpyege.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bozvscym.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mlqoiakf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2avnmnrga.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2croeqgly.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cnrtfvnt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jdmnrsfr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2knhirxsv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xyhhxort.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fcfjxcsq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iviriraq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tarvrrho.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yrfecqzi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rmwhfqcr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ekkjcaes.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mdcbsytx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tncgnjai.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozptahro.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2luluspms.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mkwsilwc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rhtiknbj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2piddwmgr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mxodezcs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lqregpwt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoedoljg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xoxglwhq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2phugydno.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mgwzaqrw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eynumifj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zzkznsfz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmwkagea.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aawvgvlq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tahusrzh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wjvgnplm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2srogjlmq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lvomtevk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wgkbillp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2njvyrveo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jqptohau.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jnqstqia.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sektclyp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2eaznaejl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sfrkqtjp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2quxgtwic.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2poehkveu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzcrpel.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vrywixjz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kdbkgqmc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wrrdmrpg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fzxcxmhz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2klvnoafj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2euovnwcn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hqmpnhme.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pstkzjcx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wylbeuju.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tfvmsgqy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2stbinpig.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2plmuhvfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijdqcbnv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mebtnmru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djcgqvwm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cssybexc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uhtnkcng.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pdqcznqe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ncyjzxzp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tojunxwk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yfwokcyp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ljfptaao.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ieligawv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bdsibsac.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jxyqtoob.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yqcjdskb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2irobtuyp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jafojasd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2asskjzgx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ublquucw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tenmdsiv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rmgxgqgp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ovfpvdfv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2voowtrlk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2srwzzhfr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nvcnnzna.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tdtgzffx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tsntgbuu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uzqplzpb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mbfeacao.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgibuobt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mocmyuev.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bbjybsrs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sjelrmga.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2enaqnotz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dmkplprj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iquqqlcz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lfeaxjdl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lrvpxgxs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pcfsoxep.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vfddswbs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fwhaozmv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wtyivgaa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hvftfwfj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2biueicbb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lzbpcjeu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zlzpmmqe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2svxosmqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2izfnshej.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2apgumhmd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kagfymve.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yumydplj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gxaefgwb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yvqfjrxt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rueyoyma.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nkfhnzgn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2quijvswj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2etgecpaf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gpelqwev.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qwgqormc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2drnqohaq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bpgjlzcb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vwrtdoca.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2byqwvqwa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ilfzfldl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lebriewe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gkhockfx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zytxiixk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qozwuzqp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2duvgxbql.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tjazalsy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jiuednmz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nnlvnckk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2oddtlpzq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2nbcwiydo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbyykkgq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ushgdfor.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dpjnjkcn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nbheiubo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fbldodjy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ajkouoqm.html


<!-- 参考信息 -->