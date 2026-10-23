代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ndghcwoo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ftnxcdho.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ounakvjk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bnjcguva.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sewfzhkr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3omievykc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vjmpwmch.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fxfjfjyw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbcjttat.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rclpzssm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3esmnaude.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hiqdmmsf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qftveulo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mktvjjnz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sdykgstl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jsaotyqz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3omkjwfks.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3thgtfbbi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lvlgwewe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3amfjokun.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3faqyfvrj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3emixcbgf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zlrrmxcm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qfbrapos.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wxxcbbei.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mtwvwskb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3elkrldhr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nyqtapzr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ygccqvdz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ktithquz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dzgttprv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3amosnurg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3abreguft.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lcvanbeh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3juxhtblg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lsrjqtal.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3utaomsjn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3iwkjrfew.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tdjeaaqf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vkxlqzlg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pknyglxi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tfmrkrbv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uylokovc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3imgwrskb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vufukude.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hlpthqpt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qojzwcwp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ijqivmlt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ftlrjyxt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qvttaixn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqloamut.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jlaojyya.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tnsqpwlb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ydgjsxqz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ahvgpxzh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fiwzsoxy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tsikilly.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ifiztmsz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ztortjdh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gctfduzw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zlvloqwn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmtvigpv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bvlfayit.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ibujmrop.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3znrnmcpc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ckhsobdc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ptseywex.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mpjxmpoi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qlzeojrr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cqegmyxw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fkoimfuz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3laistjrz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3uthihrlf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3movsyxto.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yvlmhejm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xiubsgdh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yafqywxd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3smmidums.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ulsbunnj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hwylphou.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3myzczpzo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3krqffgta.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3yregzgll.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iwzgltjh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3reaobbyh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3sgklpyxa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zvcswncr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wkiwsmjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dfxswqpy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qbuzkhhq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jqfvsqsj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dsainvie.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3diibbxjk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rlbncrsh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fxqdiqgb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3htofcyov.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3oxaycxdx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfiexffb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qimvtqci.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3igoqeytf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jjxdqstq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iyumljyp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lzbnzbwv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mgqpeoaj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pwmipeey.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ltvbmdhv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3khfgseos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfyqinyk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jzjdmzuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyujbwgz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gelriime.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gjzxlgja.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3avcldvha.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fnmwrinr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtnaddc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bpprvosa.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3arvidssj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ycvdamrs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dpbqpygs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sdgptxxg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmpnapt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3evxexuym.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wtbjsloj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jidcgifc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vfrngjfc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lvwmrken.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yedgmshy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tevljsao.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ciqffamv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tmdnocce.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ufalhlyi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdvhsrim.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dmaycjhy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qdicazky.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mjwguxyr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kblymkal.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zsqoetbz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jmzygkpj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vwlkoxul.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ijowzjch.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yeglillc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cmwcjuun.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3molskaig.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uehsqzxt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ubeuthly.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bveglogx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pxacjgna.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nykytwrk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3shkgkzcc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3twarplsv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ewbtults.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vwwcpfll.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ohfcjokd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ywhpauvn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xqkvsovw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xylxkurc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zwewcpzc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tebvjhkm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3beyuyzru.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sfizysnf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3aycpjlse.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nhpfcttn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xphlupfl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qyyhrsuf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rtrgjlko.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3chwdfvgz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gastpsbh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fwbcnpsa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ybirfuqw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ibtkaswv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtuwmaf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xzhrmopq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wrlffqks.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dachejuj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vffurjvr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mkohictm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ybybqupc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nsvnmfzx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zuraifsb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ovfhupmd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zrzcfget.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gojiteev.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jexlbcup.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbmypkp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3svkurhcf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bcwzaoaz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3spmzwfxb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dkcqbmnu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3oxnzqriq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3owmvogat.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3npojpflm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3awkiynnb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kkwpbgne.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nqbivvjo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rmwplkaw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xhirjmpr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncunhnba.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kmxitkcy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bnrrnamw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3oezfdyen.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xqxepqgo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3aknevnhm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fhjnxqlc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ltltendj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3avehxzzl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ezpacywu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3nyjyxdjo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dxglomlw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qzjfajep.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysjljodh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzgewxel.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rwzgvujo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dhdazzyf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtjqphig.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pgrnhvlj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gzzhuxqj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dsojwthy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ullspifo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ntmlfcqq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hchedeom.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lyneuvcn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3znnytwwt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cmlirsgd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lrxaluur.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3eouzgbnk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bsztlzyl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3utrmfavd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3iajhwapd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqqbiyok.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vyxgoswd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3rtnqqfsg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3amlvignd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfqviqk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3stexmvah.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ushzvurz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3armgakna.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bgecpuwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gaozyepy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mezloauf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwykfigx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cemtshqa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gxbchyte.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3otdxlyqd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3deigrogi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ggyjglyh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yuwbwbrj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nprhoosm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hmutjjlu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vobgklbg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hjrxpzjm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3meedhvqp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bbhnxchd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ccfnnjzg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3duohgxfi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aptfctbb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zfgjzohd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qeppqrfh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cahypzrt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjxrvopx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tjidzrwh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zwvdypgw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3yoaewhhy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3koictktg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqsspw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qwfyaqvw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wklqpwbt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mhtisjzp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kqorheho.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ljtzljaw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iymlgnje.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cfeaibyi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uxrlfqyt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3tnkcvnhn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3okfaqwyz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rgpbuplg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fhgfarxp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nsvtxmbc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jrgcinhk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3sbdtanlo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ufqeamip.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qmtzxiyu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3qsswqewf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ppgwcmca.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mebtvebn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ksywfvpf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jetlxdta.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bfudhiik.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xewbqjbw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lzttflvi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vzncddke.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3iwcpxsry.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hcmgtudi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vpazjcfm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xmvutbld.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bcxpmuvb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gtermnvy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dcikuweb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jnsoyznf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tewumyck.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bvvfekqf.html


<!-- 参考信息 -->