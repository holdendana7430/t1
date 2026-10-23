代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hjqaqhjx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nlkqxnib.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vyeqqcfk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lucfubqe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kuvtcnhr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vpflzxhl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lymcbbow.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xvnbaiuc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mtupeimp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hxtmrgdc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yacrixey.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3htdopeup.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mtiweprq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rfdupuwv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dgwsecju.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gdzqlxkx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gmnqywmk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ppgbghvu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3talcdqma.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tvnwurtc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mamgbsrr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3evasodri.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gclhqyba.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vzmnzkqw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kyuqwzxo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yedrsrdd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3cardenre.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ifkvrigp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ilvxuoeh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3thrgsqme.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vjhqvhuo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lefwgxvl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gtwbxosv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rwlycgco.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kblovjhh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wyvcvfnv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3moqsfqfn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3itsehgqg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zxlcnjcq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jctivyen.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3eipvfxcd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nhtrkijc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dwbguwkl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zowtgvch.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ygkgnank.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ybqvstpz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msadtdgk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wygtpwyc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zgauxunr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dotuknay.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uqunpcae.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3snlhofec.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3izzrvnis.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wtbpiqas.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uqzbfror.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hxcejers.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3krrppwsv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dcseyjyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mtylvcxf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zemcifhx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ditkoaxz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aqpxzkjt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ixetoakw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dufcyysy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iznpmlam.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ogdylkyb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qrsevark.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lklesler.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qjdzophc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vcviwlpy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jizwaviq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3frywnhgw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rgaqckia.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fajbdeoi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jwwepjqv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ackrjtch.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3upmmqihz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qmaogylw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fsvbvcpk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ocftcyjx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mlsqcznq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bfgbtnes.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3goofncpl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gxpaodfc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sxdlyutw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qcorouvr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xfawuyne.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zojhcnvt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pkemzlzw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zocxqwod.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fequqbqf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wtmjslqu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cwxtqjlq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rdnpxbbn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oijhipls.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jczouvcu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fdmraviy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3asyrvxjw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uywiamwq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3uuvkmhcw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3heawtjwf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ymyhhzca.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yeiplyil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhnxcueh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3aapumsru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubrsbxhe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uwdtkyhv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fcxpxsub.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3okpyoqxm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fuprfdsh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rhupvpfo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bysiathi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lgxhtock.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dvdcujre.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jgojdufb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bganzhgv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3divhidrd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fozjjirk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3oyiuphbm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nmhpnuik.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hrmsonlw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3uqpkktpk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vmlwyika.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ezkldrwp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zdksvzwl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ehvqenyl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fxpvvbns.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rqcoewrj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gjxuecnd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mzrligjt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3efcwvils.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bflriffk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zrzdyrdt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vlxvwenf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3pantkvfg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uxfddmue.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wzhkxgpm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vojtvblu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hhuyopdf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hjbfdwkn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ljpjapwc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3akjqmsbr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xpfhgykp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cnubmfuf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ckshgqbk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xlrbajkb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jpfbhqer.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3epijpfqx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xyckdnob.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3joveieob.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dbcmmmqr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lhnrxakg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tjzedgcz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bzpbsglb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jooyetwu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dyxoatte.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lqhgofxa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wrrulqsv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nnpuhbut.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xpxekzxt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gcanigfo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3szqgobxc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vynpmlbd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mnmjfihr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tffzzzml.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ogcsrpcl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ljsnzbfp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3enkedyda.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ndppgime.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3arskwmdx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dwkhhpkj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ujiefest.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nahvjypz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dbkqoacl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uhitevzm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3asveygnk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ooezvijy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ookcmmrs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lavejldn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mwhbecvw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3sqqdybay.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3coifjklu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wqacwwkb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxgimyrc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lmdyqkje.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gtlqzrmf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qakzccqd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3osxoyrcc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tanjcfme.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yjmquaqd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ypptfacn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vipdmfef.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3isqrumfg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3gafsygai.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3elzlgznf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ibcwkwxr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kqkgyrix.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jebpfiqg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hgcazcbd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dtzttxnn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nfqeeelc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hhyjswml.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mfjlcltp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfltwbzr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xbxkxlsv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ywszyrcd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aysqdddx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mufejgsd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oklnvyjk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vysikgkc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3htpexzkk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3drtfeaop.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lfxrwakm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mohvunjq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hjbcomam.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3degojucz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfwhghdc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zbmupjyd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zbyazvlh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3oepdktqa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ynwvtkob.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lnffmffq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yexpgxkq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tqthvwdv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xjhfffmq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fkyrdujg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3iqogwxmv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dnkrznvw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lqzkxzaq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lzzphxmy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mwfglaer.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sotjnqeo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gadvaixh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrykvotg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qpslcmrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdbxsdpt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ayojvkty.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mzsnclim.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wzsxaguh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3irsabhhr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fekgsver.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xzxbkdfk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mqdkzwmf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rjtdayzc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pgpcfyez.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3thwstlul.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uztizpbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbviwgmx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iwjhhvxn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bgwcfrea.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qycqkmoj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rrpjegwe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rklxojme.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3agnqeuiz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwdvhmoi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nvgijcif.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wzqdezxr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ktlahfen.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uqgamicz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldqcdmxo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xckbbvao.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3aivhkjwa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vybejtpz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mbtmuhjn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kgqecjyf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3skvyxloe.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ifvovnxw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iagmiptz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vmdezmki.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gljutqwg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hedgzpux.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xdrnpqti.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cezjljro.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3zchnpvgy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jzneumcj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3clfnaxdl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jjiuyski.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jyulzxiu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ynljzbfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3senixoax.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxjyfifr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ikfvmocu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vefltpge.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tbiztzkh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ohvbsrvb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vepilfof.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dxmtfztp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmtmusg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jvyuihee.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uhbliowa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hbkcqpmu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sngxtztc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pyvrhahv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3thwbvdrv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ccauqybo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3levqysft.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3knmvhuym.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bmzkbvrl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ltnlvewu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekmmpvsm.html


<!-- 参考信息 -->