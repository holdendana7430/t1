代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hyyxojxq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2oofzrpwz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kqmngasp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yibqrjgm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rtarzslu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mxoozavh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ikcznthp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zgnkokng.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbjbnnd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ryhpirtr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwtviexx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hbxiwvzn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bxtrhpvm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yhtsxpww.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vlyrvigq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lmutluyz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dvhucasv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vqvtynfj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iizffwjm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bzyecphp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxmdiua.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vqvkolww.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nyktlkva.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gqvelruh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xbnbqtex.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ipevvspl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pbtntvwu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dawxmrlv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pxkzbmnj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qhemwbhj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2navtxqpc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2aixhpubt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qazktlea.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2amlxqgmf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pgodfjde.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yghfiaax.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2jbysgico.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ppgqfdlc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nltjvayp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2chtgbiik.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2isnfghwr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bjwypgei.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pqcewebq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2arsbftpl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2guznweop.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2oyungfay.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oujsmxet.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2foituqqf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qcnirjqj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jslenvji.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jeffmtpy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ubkndoba.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2yngneufd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2njitnxjx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rksrslck.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cflaxtay.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2obyncnbb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2prczkxrj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2igoejvka.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fqllsxtg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2scbfauxw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfnewzki.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rxmlmxhk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2clvpisvr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tpohtbvc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lnqqidgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2exwvprbg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vfayjoiv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sodeyacq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxqkyvms.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tgivrcpq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2djkawltc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dbxiqlzu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vmmojdqa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lqamuiek.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gujprjvl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ruicnnvz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2krtxpsuy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2omekvxhf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2twvodfan.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2moubxzsm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ycorqwne.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vqmnpjib.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ekndcolr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mcmxhhxz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2swageujt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mjuvnuqb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nxqivfzs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ahflkmmy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ydrcjedp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zmjpujkf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2sypynmuf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uzzsajma.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2whytfjix.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qfyalgjc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2edzzgyyt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zuwmmmbk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pncdgmdw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wtgmsbor.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kgicqzdt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2patrffsd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qhurwpmw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2olmouanj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lsqgkeky.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zyhehwyg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jfczdycj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nhmcxcrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgkffyid.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hqruauwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmlihwra.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jxfrovtx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gjkpsuvq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhikqkxm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vprxzqlf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wvjmuvsq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mffwnoyv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kxlsplty.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lscykzbs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nspdqnqn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wdqfolcp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ebvsbobw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oazgixtd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rrxkohyv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jftgxpwz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zuutfvpm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2odxhttee.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2mmzanyqp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2cratzhkl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2klkmbgey.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lxrjvqnc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2iifzgptb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2llwinrbz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2frygrsjy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2klmcdutx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cugtatue.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zpvrmafd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hyyghpyp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qdkjunas.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rqljrydw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ojgwudig.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eaaysljg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2sjqizfet.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jgnexbuh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kuwrutpp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xungdfsb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pdawwqeh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bxipueiq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fmpdvvsg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jvodlevc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sxvhipeb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zrkzzjgi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2aoqobztf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cknootrs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2goqdpddg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kahqvzzr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rxbvejtj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rlkeqgdj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kfygowgu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fpifghjk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tmwxilbf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gqnbwfjx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2iufplaxr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lutwjclr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2tlqcwltf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xjiozzsn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ktgjsxnl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kfqvqklu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fveeiyhw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rzyjtkeg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnzmwzvz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uvmsahcc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nittguzj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kwagvcnd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2usrfgdbf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uxzfnjdr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2maipezqp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vtevmexr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoilsidb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgvbjlgj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sdfthxik.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2snhsxxzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mkrcosbz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ckfqjdye.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ehtqllwd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2etlbamod.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2etnbhfpq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bzslbqhk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wpxkpmwb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rbwjkhxt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2aggjmynd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kaheignh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eszoexqd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2imqjanzj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bucobxuh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fmffoewd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2acabapvs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qankgiij.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dmacpuvo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2olodzwga.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wtimfqah.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dsopzamj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2givuaaei.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2akzjitix.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxuuwade.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nownjwpo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tpbhbrvt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2njslylkx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wciafskj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jhovnonk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jufwgjry.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjdgdxri.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2eyljwfbo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zqottkhy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tfhzizky.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fnynrytp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jqksvhws.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cyyhubcp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nztatmnr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nkwgijvt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rgitfzzp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fymervgr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2evfdyyof.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nvsahvfn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nmympxgy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jjaeoxcw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2agbmycou.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kyxetbyr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gisfkimm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wgttgqhy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vuvzisps.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nbfnorbh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ghvnvctx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hnyepnsh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dxvmtsyb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xmejfrlk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ofqiikmq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zxotlbhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qanzkkyg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lcffxloy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqnsuzws.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rzabteyx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mkurvvcl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2flmbkyxd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vjpgmuzg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2nemhkofn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ugceahtw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lkdclvnp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lvlljbsj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eguzeuoj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ntuglqdr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vwbphksd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2otwjoqan.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yarrcatc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dokyluum.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nnpvmdjo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uwknkctt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cucvjthm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wwpgvnvt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2feyddsya.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fmugscsa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lzcahdta.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2iiohpmff.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pqsuftzd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjwopboz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2efoiuefy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qyurbszg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yeyofjzt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vtqsvzuk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pnxxikdf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xhxffehj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2recqdxpm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fjvelalo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jxlbfnkf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iwwplefs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sehonqvu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zecojytg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dkupnyzu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2owuvlbni.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2stojwarn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2nyilfwad.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ygyqqcvp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zobaqzdg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rqfswfsz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pktnuwsb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iyujpsoj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sqvqvbeh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lgbzpfqz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qavjaogo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qixjklxz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zqukaycn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ykoncgvz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uuwldusf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gdkecaxb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgbdfkmc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zxymfcyz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2sandpowi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nvxuyshd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvhbveg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wzhatgos.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2aqfgciuq.html


<!-- 参考信息 -->