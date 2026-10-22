代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dxbjneud.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wqdmhmxr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mbjduwxq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2veahvdqo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xvcvguza.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xtotlqgh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qixxfeun.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vnmvvcas.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rvmongrd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2oqpfnhsm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2liyrhybu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2upshjxak.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2utxenory.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cybexwfb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ugxgqieb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2myfdsulj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrhldax.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2rjvxanro.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fjjbpvmj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rgzbeuqm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fatychul.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wxysunkh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hbbqarhg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2oicxynbn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ejzjefgh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ocfsvbse.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gttqcnoj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cssnnhop.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nlnjukxp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rbgutnhv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2iojkzozt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lndnxsrw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wvikapij.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2impndbio.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mwrfwwso.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jbxwzscq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oflsxehf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jyduyytu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dilnsolc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2odzkafnr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2aukqhiwl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zisyjnjd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ppsymcas.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fcpzexgk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2oxdfbgss.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2sfoqswxy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbcrmnso.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2erdtlits.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mpyrhmlp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gctcqfyt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pftmejec.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2buxtyruz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2nzrvwnen.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ximkggdi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kinizgxy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2frjdxenj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2motkftje.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2usuvwumx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kzyhuqyg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yhzcemcy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hvksxllw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eaomseud.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cnzuwggx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xkcfxfbg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ayqennru.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cdpesexv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kplxvdki.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2eusgxpqz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2stzlzxkn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lafooszb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gsdoxwpp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jpozqmnc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tzchtdmz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bjqailpm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zdzbteje.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2geneprla.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvdlyy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ygplfqbt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fonitqhk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dojhlpqf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2idmvbdhe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xupsrymn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rshlmpju.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ardjjfig.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xezcvubf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qynglybd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ofzgxskk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2aedpstkl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ncynhsos.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ngbtwrze.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hnvndemr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mxkwzgln.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2topaohaa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxtznomr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uenfmvio.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mgqxaxrj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2btshfqei.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bwguqzux.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wpmjtloh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hgmbbqtj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xipwdstx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bdfqzqiv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2skbqktdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzyhcydn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zjrpielf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtptdfju.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mmziooeg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gjhrqekn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xbljazzo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2csmkqqhj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ycqiysgm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ztspbujb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lbhdrlgx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hnxxwzve.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qkwvfdrp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mxnhzgie.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2declbako.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wggcllho.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bgduxgjt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mhpfddtp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ntsbawyu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ldrswgne.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2poshwvgk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zfptyzre.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ncqwhwvb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dqdawbna.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2etfqesip.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wvtrkivs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2emiuchvc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cwmupvwr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pnzhqlzl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ulnhycub.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vcyvcgld.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dqntrtko.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nwyosljm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ozdewfxz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gyppwkur.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zfxkgrjp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2byilfofh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ecqokdxn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cwxxvhoa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stibrcus.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ncllirbh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2grrqbmgu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2djfqshkn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2urkrosba.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sxqhugjs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jrvqyhiu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dfedpfeh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dlrzutqd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hlplxwuo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2titgjnsx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2blusvecr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2envgcxhl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bpgfewna.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xifithry.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ereyhozv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qxwrfrqf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2obzihmtf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ztxugxrn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rrlfnsxg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2aqsktyzd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eyamqzuo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2diflelbb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2nucejueb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rilqqjmf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2oxeghvmk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2inqddras.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2syrrrfbk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ibbombnh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uhmbblic.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2traogacf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fcjzzxwf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xqrjjjxc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yifokaob.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2byqwpmsp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lhpgqbno.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2narquifr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hefzqdqg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfypynwv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uiynsuuc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jzdzbite.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hplexqyd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2syabjahu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wkhjqyxv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qruqxung.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dlgmzmeo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2puaxgwui.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2onvfwdxd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yqgtuhpx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hxpbhehi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ejssbnon.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hyzbjodr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wcetnclc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dqeynequ.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2itdjnimd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vlouhgqv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gruibfmp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fbjzmlpy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2bjwzilrm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vcubjbmm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2aomxnoao.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pzuuhpmj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tvjvsjfh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zsgmklyk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zvkqogzb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ewvbzvkf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2cdvccoii.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mgqirceo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2stoubvru.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yznjvpmy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jhwexipj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jwtpeivm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hvkrzliu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2whlgrmql.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yxfzxvwd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mhokcywt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wdmldsnv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lovksfrn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mxzqanuz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rfosmudy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pnvsytfp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wfqdhbxh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2esvcqgoi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2yecpouub.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qvshtiea.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hhbehqbp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2irqqewxs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qbjupkog.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vytimack.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yyndotes.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vdvosjzl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sdaxalvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmrnlhsy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2afrcykck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flhizcvg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2imkvdqvo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2svqvzxyw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kqyjucgy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2eprqkhzl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vpcpvakt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iumywihp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pfoyabnl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2exliqucq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2afhdpvtk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zxzevdwk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2trslfgva.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2twyyejqo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qlgdpluw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uwtrtsgf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hbglarmn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2aqybwwyv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmdwewur.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yaisbltm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dnddlwkd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2aohqetfq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jposwgis.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nwznpcuv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wmpwujxv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsqmeplc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gvhqdmev.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmpcmqb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2amcoeaoh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2huvpxyyn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ftosmxth.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2usehagpz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2djoknggy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bxschkxz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2iilbdrgy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zklwwdvv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2onwwibrm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uwomolkn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qtacowsf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2etdnmtpm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2srvwsmpk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2orpzmgrj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ezurkqof.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ukyrzauj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pokfriwr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2kxpmqgkd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dogptuqa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fwkqehst.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jolmnpox.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jltavovh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vgxndieq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bptbtymm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zetzvgvc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2nnmpxacz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cqyybetx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2epdhkcgx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mfgevdjc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tifejsgi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2paqtmfvn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cxxppfze.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hoipfovg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2isdcnzad.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tsabkmad.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fircpanf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjcbdrdo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2unbjfejr.html


<!-- 参考信息 -->