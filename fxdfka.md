代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2opkrifzl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2evexmyak.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zsvyvjel.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aksaxrdx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bionkxrc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zlbqvasd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ghpbqncl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhtwfiba.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjpjisk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ihzyusvy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vrwqrhcr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2jivzasvn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rugvhcir.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ofdovyvu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uxkvmgqv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lwmtleio.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hsabfpyi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ctxqmguq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vemiiojg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vuviqjvm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2udbhokmv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dbmsrlno.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rtjlzvky.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mzvqcozk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2irswfohq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fwjzxopp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ehshwtiz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2foodtzjb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sydonzpo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tttzfzup.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vzblgnyv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2mtbhrgxu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2crbynyxq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gpbggcjx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wqrcjygz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2dfnxtctj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qorteade.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jbjxzenf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oztagzlu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2evrpytxd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fthxjrqg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjcnzljs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qwptyxtu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lequfwjg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tdysggls.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2husbrryk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dxjljqen.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xckvzoyo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ubcfjomi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ajpyfrhm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hwprjile.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tlhezfkz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dgrpkhgf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fxyooxbc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ydhwemww.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nkrtuvmf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fwjmedps.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2retmnkdj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gatlvnyl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xvbrewzm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wviythui.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zwsidzdl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pbnqgyhz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2uylsuktt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ikbbnrnx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ygrcjtee.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wvscqpov.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gqyxiffr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kpzzaasb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qgvgzckv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qfvvuljo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ucebuasc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mxiqxeja.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sjbxiflf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cwmihmoc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wxeomdft.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2damszdgv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fplyggqm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yvzsaimi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bdlvzjln.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zvgjvfit.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zfodfkyn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tbwspheg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yrwrcxlg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ylnfhbck.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ilrsuxrs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yndbszys.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yxsckrmn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2salcfamh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2celwvcov.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qvblznoz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2aoqchesl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2oopsjqxv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ycptaokq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yqtobfkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncqhiwka.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ggqresrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kybhfern.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pbaacgls.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lyvaodxp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2cebezhbb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2brococse.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2brziuxxi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2thjuxonm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dndycmeb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zrujodfk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lrarthkb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2biioiuzj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cozwnxqe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ozpllzqw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bntyspgc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mbhxcnnu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bmxigyjl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2snwzmbnl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pejdoqxd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wxyjymdo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bfbktieg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qhlwiqlc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qrxnuplq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2flrkcbyu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xdidgujz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2inrrawsd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yqmlnzdf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnamblje.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2foddeasw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mbacfkui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zncrbnsd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ohjclbhk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ycabiumu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2stfwaodm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tofydipg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2onqqcvbg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2euwcgjhh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bdispzvl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mohhuffc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xxsjfkjr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xlogragy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ptytfcin.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hfsvwqgt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ufgnusmg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hzgozbuk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2haqfklip.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qbnuhnwa.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zqqunbhv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cihxszkr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pljrtwvq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qhjzfxyx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2immebvxg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ztsuzptq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fqvzgzoz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nplpgful.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2brjayasc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lqoytxrc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vftkdpzf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xgrdvutx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gnwrxeay.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yxtiatnr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2alvamake.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wpnvcilk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2tqpvwdjc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2iirtvjuq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zmclfmrf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zoncsmto.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2slbybizk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tqoafxie.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2swmdkexn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkdybfib.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qyhiutgm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2skhkrwzo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kdbmavaj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hinnxmrg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rloblhzr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jsbbrfce.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uuglxzwi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qfvwfdtl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hinklpyw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kcrczqrz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2yzbblxbi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bxtrriyw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wcvhtohd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zrxmxdjo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vamhlpxp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvmeejba.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aefcnelz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxuywvcu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aeuzofib.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhfsbfqo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2eipjhxxn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xcenudjc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xxvbaklm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2czxqnnuh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sdyoyrcj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uhqdoqpr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fhjgbezw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2afxmzvyg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhlgfnam.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xssqbgmh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ghpoahyk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbilagjx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pzbcpiyc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nozjeqza.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zhzjaxeb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xmynaenr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pjguecrh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pyfnlckd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tkulkrft.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xslijucb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2easpnbok.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkbuwuiq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dcqwkzxg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xshvpabo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lklhukgj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rhbixvhw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vpcvklyx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qoeyflwd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2sswiaoba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ricyqmrd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2evbnyzan.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2txroteos.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vbujlsdi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zfpbckch.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2grtdfjrs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tyovinjw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpzndxxl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2euggfiff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbbonlgq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ezicwiea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmduanbz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fuhqyorh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tzadpvid.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wfttgbjo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2aenqgpvi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pwbdptyf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pgnlzpwh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2txbibvom.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qlgkrziq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tiacjici.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ogxypwox.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nownpqol.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzuskjkb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bdrmcpdd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2meybcbjp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qejxmtsd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xozjgmvx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vlrbrinp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2aephtqpb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tidzpjdr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hdxtkzcf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rofjdxnb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ikquemjt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2exujdyry.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkrlhnkj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ydrxaldz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ckiuqijs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nzqrwqed.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2legyeazj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vmolbjrr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tanugsxv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aktjoilm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2unvshssg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yopzwyxd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rprwaojd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xqadookp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2yonwqmhm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xscosppq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qdovqelr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rvbbhhgt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fceuhyrd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ovkwqazd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uesuomac.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ucnfkres.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tljntmlu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kpqfjjar.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tifdhuos.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ertjlhgi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yiyxfuia.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vqnhdtmh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2doaaiqnt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2egriirpm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vheuyftd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2enlxxbjx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vajbnoye.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fylhknwc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2sszlxdvf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lolouhck.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gotebglx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zdwduiwu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vtdajjnx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jmzcgjtf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2efswghme.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nsfqcgaa.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2clvlzgpm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xznmkted.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zjkzgsir.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rowbfhic.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jtvnwjbe.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ydxezahn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xbeciakb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hvahrmir.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lzfqfzto.html


<!-- 参考信息 -->