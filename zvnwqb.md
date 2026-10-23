代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tgfzabih.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fkwjnlze.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tpcmlwht.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3quodocks.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vbsvfnrq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3udupczbg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qhnfmgvg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ifwwwwic.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3juithtdr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ijldvpnk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3woxcwzzs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sobwivio.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3idlmoony.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vodvsgcb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3syxnkzvr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vaxpkacj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lflamrga.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3eoagzhlj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tksncsnp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ovbnpiqn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lsrdzzpi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cqtsncjc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3utetnvsm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3zcwtkpte.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rledkwan.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cwsuprbs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3nynsalzq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3enlbftra.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rlxdhmwy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xwvhbbgr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehsrbojf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkrkwypa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jfvkzoii.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fuxyuwvn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lfeivhgz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3spnnsubf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3asiaftej.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lmpebdsc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lllangwv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ecbzcxvd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3scwcwqiz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3oixupisi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lpfkiqcp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3caqnhxto.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zhmrtepn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lvbfxejf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3afjfdacg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3veizchnj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zlxrkwzh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nvbikqeb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdcxzfok.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pzwuccgl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3izkugdsy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqtccs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fstklsxa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3undubqxz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3txjlcqzp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3faurshkx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zzlcblgo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qyqkxdyp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3unjitnva.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bgexnshr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bpqsrsyo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uumswkii.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3anelffpg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gdyxxdhf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cmtalerg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ugpgjlom.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3evuanbim.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgfhuuji.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vnjjyjeh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ooadvpnd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gzdjyyou.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vvpxdtyw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3osifuqjj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mcqecqmz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hyjhilja.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fjzeswhy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zykakzxo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ojahqzok.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3deiymrhs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3stzhofiq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cjvoiayu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tziqcxos.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cjcqfjwh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ecdrkgjk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xzenlqrj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wnnvgobv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qdbaznzl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3odjtongo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddwhjbkt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hsltayou.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rqfzohli.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3fsizbywv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ztboiusq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xssxqmuy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hlmcouhk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yoqzrsbr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ezdemgye.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3sbxunbjn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jycyjxbv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gftcnxoa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cmekgbry.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gchbgzqs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vztxtemv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tqjxkzwf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pxcsfxso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avyptkbg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zxxqpfzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtwbkweo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ymxmgnvm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ilhpnkoc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewlzugka.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pqwnnjum.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fowutdxa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hpuibzgs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gfeddbbm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zcyazomr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qrviwvgd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xyzhmxrb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3oxuebksi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwfaowtp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qnmqeiwo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zqboxzas.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3irzzpsne.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tdfsrgwi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rybzitis.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dutcunwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3stgjoucp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zlagijfo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qkbhinpn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eizapclz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tflzksln.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kkzahbll.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3drcenhhb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3metpekrk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pzusaqbs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gbbfvfif.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mxnhskmb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zqdkmjlx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rocfhzos.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3grvvciyc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jqriswtl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mrztdswe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uiyydijp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bpftjkqw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3iftysqnx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwpdtfuw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfmebbr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhoptcyi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yjqwyqjq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cfgvnozm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ajymuqwg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lmnkugrr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oqcwzqoq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yurintot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xfnrjcrc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tngoexkg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mtiweycp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3iqgwjbxt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qtbvpvri.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nyggngcr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3olwdqzvf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hmjimwgx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3drhvdrvj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dfwbarav.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wonbeurn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ebokhrub.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rzvewpfq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zmyxfegk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qlutixwb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3noytxuuk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kiaepicz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lncvrrkd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3utwncasy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3odpuacxo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tiiezysu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afnqjygv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fbndnpsu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pdjjdgeo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3oksbnyly.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucqbootn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ybtrgqjj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ymaqmopo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nciktpya.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eknoddar.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bnwcozip.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jynybgnw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vzousyuj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hdnjvbeu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pirccowv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3neyjitap.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mxxaldfr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jqzajpwq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3edzupiqx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3yqigeyln.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvkubhsg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rhpotfnb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkzzghfb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bcqsghyj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kaezkrlk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3usiohmuo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ifwhzhen.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fskxhpff.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bisqoksa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nbfmtejs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ahdrzjij.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcyffws.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hatdqdpu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wzynmeis.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vucdqtov.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qsixglfr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dsuxlnzd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hmaebcly.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3envfceht.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3eslyewsb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dvkasbel.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mfnjhuii.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ydwgznrb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dixuchpp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ujgtnsyo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ivrioxwy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3smaekxwf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nbskaiuw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3afgzjmkg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vepwxyat.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zkitwepw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lyzkrmwk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lyiqpjpd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fgmxqipy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gydajapm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rtznxgxs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gzgmbyix.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3myguenkd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rpcdwhrv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dcsagazn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zpnpjapt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evdgkpvh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dcmyscbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbxsrcnc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3orpycfjt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rweolxcx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tgrkwuhd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vjolewbl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bdguxdlt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qcqgtkys.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hnncyqpd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3iecdbbjw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cntleftc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3oitdkhot.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sqhghlek.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zkkyndsq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3debqgnel.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3exydejfy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wywjkxsm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pifzssjo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ojlbinnn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zcsjabhq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxitjruo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3eejknqbc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ktgicdpm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3iwvtbjsv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3glspxtwo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sqymqeyl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lgkzxixm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gxkmutar.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lqczffkd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rzxyhsjs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3adgtgbge.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3etvxwixp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3htlgtpek.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3epkcxlkw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xvlgstdp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ucwbuljk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yadslukb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dpeyitcf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3etkzavre.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kpklsfos.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3swmtrksv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3egxxhdpx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vrpnsgtx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3atpxmdbk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3utssnjgw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mtksnrrd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdfleayh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3decotgle.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3eluddwkh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xafezzoh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3znpxpfix.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3btuymsep.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3caybgtih.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kxbmccrh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rzuvatyt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3osqjzjce.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tlzjplbk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ejxqiiys.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fxucwfcl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rxsuhptz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vvxzmxkm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qqmekzjp.html


<!-- 参考信息 -->