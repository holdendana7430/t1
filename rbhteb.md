代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3muemjphp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zzhybbmo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bguzroul.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tdrykxww.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vrwlsgcj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3knwcyxdc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wzpcyxri.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hntgbwkk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jldouhiw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ahfwdxqv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfbfiebl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tmnvfrnv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uzywjvzq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dmhrnaki.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sqiycidb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fysjsdqm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ulybgyxe.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jvnxpsoq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wafbifgx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3upcsxywc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fmddljfe.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kmvhywsq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wiqkvrko.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tnmisnxh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hidqneqz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zrowpdsl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hacvnris.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qnshxjgq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aavlpsdm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hkgxcwch.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jpewdgvh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pnaiuekf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tbwdcefb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gpablasv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dnahuxpu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gncozbjm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lzhlpgxy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zypsdxcz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3eaidfznz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jxlvxggn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owlwopmy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dfljldvf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3efkwyfjs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wioygjjt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hrvpyifj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zkgnnblc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vaeqyrjt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nvbwbuij.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pqpfualo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nrzfgbrl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3lwccktkj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cqddvvld.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dmxcqqdk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bmlatrfs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xvfkskin.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vkhnbmls.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ygqxanev.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ycnqdcmd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zxzzzbht.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gpagwbdj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xmemtrod.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hqnvrdff.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3htvelvdl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mqogpchq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ujtlxxxh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rugwoore.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3judretru.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3atolzyjt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zfydnweg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccyarcgc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3huydetyi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yoqomwuy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jzwyklfl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cqfrzoew.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zztivfsh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kwohsshr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tfehomeq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mbitjzci.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fuqqmbyh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hlxkqelb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vqjqsrtp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pfageotx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3oagdwqce.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yqdvexfd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ghmyqpoi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qpwompvp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vhdjvamh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hsmjvfsi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xxaddplg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iiinqaec.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bwiilnno.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vuxicxuo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xmcfedvt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ygczrrcb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ldomfxcv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cqryqdtu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3scxrbwkz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3kuwfyjvw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iguucmve.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3trzhpcaf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qpijcaoj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3aeriwjkm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3boxdmwqa.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mpqxlaiv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kecymvmd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qmgzdezx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qomeaiub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzqvreuv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3oackdxgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hiqqqsus.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ijmksuhj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qhskizpu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3grhsjrbh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jnqsmovl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dqeostuk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nzpeudya.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nhfmaxwv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3redpzskg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cgywlaqo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3szvxysrl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gsbuoazt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vjvrslsz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hlftpbof.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jpzuzhya.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fajxpymy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yikmlttg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mhibxqus.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ydpgbeos.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3umziasbu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3sfgweuvm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xpgitqik.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3spcskfwx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lgfnokjw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3osukcasi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gsjlsldw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvipluox.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qedolvem.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gfsitsfb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hynsqciy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ouendnmu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uaymdvdm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vqhxxsdv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oilqjyyx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lvgeqesf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3giqvojia.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xshyqenx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cjhqyaun.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ttmdxuzt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tetrxdwh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xqrvojjh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mufiopoa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3agbwvxla.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pymrpzld.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ltzacnxd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gfamlwqp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rytncdhr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mnxqgmnv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3sjdmhdqq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jcsdzprr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yxfoxlrz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zupstblb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3adaxmaip.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wvastljk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ssxbmlxh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yvavxoui.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3khvxkaby.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fcaiezro.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvpneczs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bbedvwlv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ykphksii.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cszyvjvq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qceedcau.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ffftbpwb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dbyiswiu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zkifnsdv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fsiwvehh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cslapuga.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bllcifmg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vgcrlztm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3uwkkoxvj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nxxwezbe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hetkegez.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fscfmdux.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gshgbiww.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bjkjqsns.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3unziwdsw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uxkbyuuh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3afdwmhty.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tstlikha.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvuiicrg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ytluanri.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gaknwfrw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nygahqsk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vsrmrmte.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3iikdhfog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oeohcuva.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufwjydrn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jwzdwadl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3iaewdxmn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xusunrkt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wkuaifxn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vzvjloxu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3skmfhgke.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3musrtvcg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kcvsmbux.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jodfioig.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3thygnhro.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdkorvuw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mvblulmk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lszwsmax.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxwdeadl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ayxixlvm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wacslxou.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cdvmilnv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3psoaemjr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fthumiwr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tckaaocq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ufyxkumr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xeybacfi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wbshnspn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxhjqemt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3elsbvssz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3thjykavr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kovozzrz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bhetizrq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qlbqknej.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vbqeuntp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3idjbccwe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cjfppdbl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3toksmwdw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3chxajmkj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lqlyeggd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3svzvqkij.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wztjsijv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3uwjknpxm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3aidxdvdc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tepzwdxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqqrdyoq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ausxwhqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuejaygv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3frzmedyc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lkdtgkoc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rzhhczli.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xnkpqfuo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zktaaxvt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yazrycpt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hrfrjime.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3nxonvzld.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vrtqitlh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lqyzkkwz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pmpqlweg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jccapgda.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lfjsicsy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vdbphahe.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qfyxvqgp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nizjdryo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gvduxuuv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wcpdzutl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zakrhqoz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vfxxrdan.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jxqovpjo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qhdvnfks.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rakdncdv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjijjygs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3izgcummh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3htcauyvx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tmzhohvy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qgnzupsh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3anqdxssv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fqyjhqgh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3edyiyudg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vojanxts.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bkkyxmii.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dzwciebv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sefhumkz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kzttzciy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zreyjwkw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ndiunstn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ndjupcwx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ohoedkbi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xrzwpsmp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xlbkvzpn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3djanwbna.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tefyqyte.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3itygncpy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3enuniznl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xrennadv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dymbniri.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bpfipwgk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nhdkrqdp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gjlmdkea.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3izuyklbv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wqwhtith.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bzmhmywb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gltqihim.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3chetxhvi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ubznifoj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rapvultw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3smhklydh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cxhnuvqp.html


<!-- 参考信息 -->