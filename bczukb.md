代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qaqknyar.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uggsyflr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iezngpfy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3iijhxdar.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3twtbnrqm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3uhznzmzn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wblkmlcv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3hotlabuk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ludnelgm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pcwiltff.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xvelgeaq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3epawvlwj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sccttehj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hziyyomt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ilqaqmcd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3utodhhjf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mjgnjbqy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sljhldwu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3attkervp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3scxlyvqp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bhabnuga.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3srfomkox.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yzwdmfdg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mvpakywd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3astcpejf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3umibqsso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dmtuexou.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kccwejeh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3psjigerw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dntkpavn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sszvbagy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wdwgrrqg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ddzhrigi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jnozuhjp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yossjqwx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oupxmdug.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ohrpxifd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vnzzvcfs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hhwbzpfl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rsolkfug.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3skrgrdao.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gvdfzjvu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gcfomraj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vudtsfim.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3hzrnbbiv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vzrklzdf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3smseknni.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3umbyehxv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kxlqokax.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3klqkcmoe.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sczpkmfa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gszdaqwz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qylzhurg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vcnawoxo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hjjtahib.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ihwdmbbd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tvgnvitq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ozlfsvhw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3chwbshnv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tinowcoi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mdjzerzx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpvuueme.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mwvqrxer.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hblutrnp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3syjdtdex.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hbwkinwm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zgqpdptq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3caihwbog.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ertiepfj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yccjtgbu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nfxjsltg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cyojkgyo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wqpqqihk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3luskdlml.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rzlvrigg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mtgpqcni.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mmnobpyp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zoclkxhs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wewlevyr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ryqvxlkq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ivuhaumk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jpxfusfw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3shiihszf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dfenqdzq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nkvdtber.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zrnfumjt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rgaaydqq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3sllvhfqa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mwvouxvg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lqzfycyx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3trcycusl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gtwamskh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xqcwlbeh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wjocibzw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ritppogy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bzxaqqom.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pkqpmzwm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mlgnkvqw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ovhwejgk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uywlstaw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3urxisgns.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kbxpujap.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tdxcuwed.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3emtsdsul.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ltiqxvog.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3djiulaai.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ifvpcyxa.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3efkieavd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3nrjapiew.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wieqpeot.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pykhhonn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3euzsjotd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3chdyogul.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kutjsacf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3eeeovggw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znxxovlq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3edmzfige.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azihykay.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xlabelip.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3sabjnfte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vlusjwkg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jkfhfpwc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wovmnkcx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ehsdxqht.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3pyowyqni.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hcudodny.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yegbkbxw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qigkqjmh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwqkfob.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ubzydahe.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vcojdzwb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sgxyasxc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rqsmvhoz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vpviznvb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tdfrctzl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dajxglup.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cmdjqchv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nxaersns.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vgnlrxuj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3shvqdyfa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3bpazqugm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3chtdmkfl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ncjlpsax.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3trbuttzg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ldqxyrfn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zblfhrbm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kzwmkqfb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uflmboxi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ruinpaza.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3oiuwcdsc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lyjzynbz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ckrdzxng.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3viogxwbw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dbbqkekl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jtplujpx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3obfgflgu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xxfhuvkp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ehvxkese.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lrmbpxnf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3aywvfjdi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gbgjtryz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mvqroxxo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nlnrrauf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ztfqtjjd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hwihgufb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ejuwsssb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rmmrwduf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ldsdkukh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wlnqmzva.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ohtojwbm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qtxxobut.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vgfcslxp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ptxasvrd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ocsfncgh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nzfmaeel.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fdezehxl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wdpqkcfe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehjxdkji.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cevsjsyk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3crpqhjir.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dbrsvvvx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wahvjere.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lxbpxycz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhkiyotj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fctmglwp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yiwkhvtf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3walssytg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3smzbbdpp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ogkvmjof.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgxfwqsh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bjdhkfzg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3opzzzsae.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cnrygijy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mcuvftke.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ikzjetbl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uekftzva.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hmiczlcl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3huozcqxa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zkzejtxj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pgzlbhnf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ffgggppe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lcqqtyzn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jagqrfkn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3icmsmqfc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3gdeaabfd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mqxfsbvs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulkpwvuo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xnxbfito.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mitctneq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lzacwjvu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wcvjozji.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkrmbtnz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3caeqysfh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vgmryysr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jsxvuqpg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bfdbilmv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jwofrfgy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwplygyt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3azleflkx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3omsapqik.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xngbntnd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xwdkqqud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3exejvwet.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gvctfuoe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ewyepjjx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jygqlqfq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hsjmbbpq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tqejwwab.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3obytxmdb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3eehzmzbe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gbmtewll.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qrcljsww.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fbqnzlcb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ubganmdf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uoavkcmj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3thwvnroy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fpmhunrs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jadeqnza.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3olaedamj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qzhmsovs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iqywujjb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ehcwxgyj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bjrmtivi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lgxxedhu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gsgkjexi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezmvhdfz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hnjxchte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaibdhot.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gdkwmcto.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rbewldyw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbrtigzc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kehtanhc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nbbqkxah.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vxpisqqk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3omhprakz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gkyjvozw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zyhzcedi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qicznwsc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qprjdcos.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rljjnsuh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nqablusj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rplpzrdu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wvhcftna.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3imejlkgc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gohblbzu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3odkawjil.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdjgaixq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ozpaopfr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vnlaakrt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xdehzptc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3epycdxoi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oeyupqpg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3prqgxbea.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkittrfq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ezkdhzlv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qtoccksm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3sisnwkvb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nlqjoojb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ojdqbbag.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gftiwgqf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3kqljvprs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fdnrorot.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sqynxetu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3expgpame.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3unqeixha.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mdswrsek.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yvxovrmi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3sftnebju.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fniksdxi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3riunqyzi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ldnflihs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qiwxgrsm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mqaxqoeh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3paqkcjqh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wsuatgxh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uuztcadw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3niierzgw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3itzzaais.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3iaszdfmy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3bzhtheio.html


<!-- 参考信息 -->