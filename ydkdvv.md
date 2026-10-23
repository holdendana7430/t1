代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3eqpfhepd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3klrqrrrt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kjdtpkpe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kzlxgibg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rlzrnacq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rdycoasv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3loanapfp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wxfpcmxh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3pcghhlbn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fyhswnta.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fgjmealq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pmbjmiiu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yvjiyxix.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3keuftjtq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uhxpohka.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3sqghrpqb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bpzegvpz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zvcqsovs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fyorshlp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3kxjxatee.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mhjhcnag.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vchxruqt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kelpmcxd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vrddzcpl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ngkdxcwv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ezlusfia.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdoqqvxq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3isnqrpdc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jvaxafvo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3funsdecy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3oiqokhqv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gboxzzei.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qqovbzdo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3apmyfcef.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wseshwuw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rpqnugsu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tlzzpyms.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3idfquqyo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bpuwhphb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bbyyvvud.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kyemfhnf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3izdhtjbr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3frorksag.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jjdabxqm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tzjuebbc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qzavfvgr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nywawsqh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3uezphlur.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wjuygrhs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vavjincn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tahljuin.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rhigpizw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zvqkkquy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jxxhcxou.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gvluuhjn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jdbvoopp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3utkjuuyo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3cqhdfxif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qivftrct.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nlejgweg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hmcscqdx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nuutibxu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3egahoojy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vstlostv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rwjrmbyv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdrnhqdx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zgaapwsh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3resmoffu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3cshayayr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xgkabqkn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kmxrkbpg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fcenptnu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yzpzmawf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mtgvjnbm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cuvrvxhe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wfnsjlny.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3keqvxgyv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pxmaaitq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ogwzfdkd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cldlueqs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zjogkgjq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ddwbcrxz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ruvrerqb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mxpoutkn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tbqdxstj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pejuhdgv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gisxcnkt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tequxbnh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mdydwedo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3upyolzbg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3duprvdyi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3srjsfdfb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zufuksgl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ludbppag.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kqatkhzq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3docrjeho.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rzwudcbt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tjnouqqm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3njeosfwc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hidzyuvz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3eiandwhh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ebkgjwww.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ouobqnns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fubuioqo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mqqsmhuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwgvjphq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rfaudgdb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jdvowdma.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3agjfazwf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oygwfrvi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tuanwbdy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bprldeeb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3iekmyunf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pinowdlg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3klnhofjl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zsxcpgnd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3irunkylk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wuupykuq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zkjseggv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3czqefmff.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3grpqbpup.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mxpgpxhl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tihpqqbw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3akohjaun.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fyycyuba.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vmvvwygl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hgssfuut.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hybphwre.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qgrpdqcw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ipceogvf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nfsrftmk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3sgzmrplu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3usdwxqdh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3oqroztoi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3thnxebdy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gqsjnhyd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ajizjyiq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdufhodi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mksemngl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fimigctp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbmnusto.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mpvknrxl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wxgcemcm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mrkxvhcm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gnjvlyqz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fclaylwn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yqllkfyo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3yrqwrjmn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fhrbytss.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kurcxiel.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3sdtubwxo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zykzaauh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tehakdgp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gcdjeuad.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tgleyuuv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cyorquxn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gnfwltuv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zvzkfdyp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jphwjgjd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jhjdmrqc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pscnjqir.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tdukrnwo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gztcrynk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ipsnjapc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pzjybzas.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zykctzes.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3yvlhvpux.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qhhcneso.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rgqeqbuh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wvrdqani.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bsjrpnla.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cpwwrmam.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3osonwqgi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dqncorzj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ipoapwej.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qrmsydwk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cgzvozfe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qbllpolh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hwkkvhxm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztdedrxi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jxzvazez.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lyqjvkqq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fggfxbsz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tzojgooo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vwpllclm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3khvvyavk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bzmjduaf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3arkzenbb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3udmlbjao.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qrbumofw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cozlfkal.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kcozcgse.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gauwqkuq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nnflondn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hedbjmnk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nfpujlod.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3taankyij.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3krkzcbvk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fybphctf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nplowjqt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dgodgwjm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cwavgdmt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dprqawnq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pdmpqoea.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mvzodhoe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hmotkvdv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqhhywfc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wdxnopls.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xpiruwmr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhdzqdir.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gkbzyfyu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3txbimozy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yerjzykw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ugauduqb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3oknpjgvo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ywdnnben.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lydkdwlh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3szqsfplc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rmtivzlx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wnxxymqo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hrshalnr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iyosrhve.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3prybcpgn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zbnrsomi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtojqwth.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xbnsfqth.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vfdejjaa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mfrorwyp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yaitynlc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hcdrwbel.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mlnjmcds.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gyymbtqt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lshrtedp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eekjvnxa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yajhmnkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuxpednc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rlbwwpkf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hkblxcrw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3badlmxdd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nnuwyuvk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yahecizz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mflfshqs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rscoajuk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tviizzvg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dzjuyvml.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bxnptydz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3otlhwsjc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nhdsxsac.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ktuejlhs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wogmpvsm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bkvbdqrb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dwxhzxvk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpblwctx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xghfvgxd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yxaektro.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jqhaichw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vkyydyzr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rttqflgt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3obcrilhj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbphqlx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ungdnzrc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oeuhgdfc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rwblxspw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kyaldapg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kvkcmmnd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3elmgfolt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqpoooap.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cibnttjl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lmhfdpqv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ebuoyoxa.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ehswvias.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3khhnhiod.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uylahhxx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jelwbecj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lnqhfodk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oakrcqff.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3efjxtfpv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3tzgthowp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ncdyjqpj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gfruayxd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ttivwsjp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ptsuylau.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fpevaisp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rfognksn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qoytzzkw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zypcwspj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ttcziqba.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qpanfirr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qmqizpue.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qkmizvvj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yllxklvh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3roegicrc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wvdksvek.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oyrlcwky.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uopkbvpx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3izdcuhop.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmliwitq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bxzbxzqn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dsyonjcr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dyqhglny.html


<!-- 参考信息 -->