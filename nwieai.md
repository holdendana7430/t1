代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vejosjsc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pybfrfuc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vgbjahco.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qhchftpi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tfmsioij.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jbvjduhs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ckdnjugo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bbqgwsel.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gwlqodyh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tmekmoso.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2kcqfsjqf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ypaqshxv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2flpeainx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zhoueirr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ledvhecy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2irjorjva.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jkitfatm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jicaywyr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkcedlsn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ssinecqu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fggrdusz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2txksuddp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qxtajbvi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vvmzffhn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vjgtfsjc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vcwobxaw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nlsmifxv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ciffnuzk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2iohyuaqv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2yvyglope.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mndtjxcq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mlkjjohz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2knyqzozk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dxauofla.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2cetoqejy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xoesotma.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2swuvyfce.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zdtxiedn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dkevyzgt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kfbuvief.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dlhmfbiu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ugzyxlua.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qmscjxbn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2pzkaiukf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rzkmplhs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pjzeuylh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qxarewuq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rwmeyhon.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjoysvaa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uuwikqln.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2waqknrgp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2imgmayja.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mcoweelz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ankmcgvg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zfianlsr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rssrlnhf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qahryiao.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kyiguqzq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ygfnlqia.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qtsrlghk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sufyrkkj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lctbhsjn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sgitvmtj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2juwurtqu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oelbzfiv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kqbjvtja.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2innnujwv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jxcilbkr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dculihfc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzffqfaw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2adhixgyz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uwtazwbw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ykzcpmkp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2szeiztns.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2riljwgil.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2owzezaxm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2olzhbpjq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zddqjpdh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ruwhrnhy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2btexubpf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fjcuibng.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jelmozkl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2soddtxtj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vndclvcm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wjlgoiox.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tufyecpe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xifijoyf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2nssgmbrj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hrrofabt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gdsonpfq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fusrhsir.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vbcgcwnp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xqyrkmni.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rjbvdxdx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uosctyds.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zizxkjrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ryfzuaji.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jaesyfrs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oohbbwep.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fsxgklgt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qeketajv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hbpjsiqe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ieagyqre.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yrpqboen.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lubpsyhs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnzubalw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ldlqhqtb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rshfcqeq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2flyoiapy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2molsvflz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ymoopkkn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bjcqrdiu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pynxlnam.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xzmccdbg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cvachylg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fugdeplh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rfyfbvsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juyokuly.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zjwysjcr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hnaqkzrb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2pazpkwue.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zispjwjb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kiivhwqo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xjgnysnr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2azxvqmhc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2eaiuedvj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fmgtxahe.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lqofcafk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mszzwxtq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2blbnvxqa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xwhumnhk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dgftkcak.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zxwakboi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hoswvhtj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fbnxmkqb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hconkuvi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gigxtsxx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dlkgxvsa.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2khoynmkf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dekqokxl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qviwrnbr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bvnagloe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gjwasclg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyefqfye.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mypmmxqh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nucneimc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wothimad.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lxfpotqv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yfcxahft.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2muwhldtn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fedrpgrn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sltdexas.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ercgfmci.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ztiizhkk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ztwdyssx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qqrccqrt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvswxwr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lqttdzbs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dxsswztn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qzmohcvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2smpkdkwd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vxrpqwga.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bmgdhrwm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zqiedkdc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2alxskwmt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yxlexsot.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cmzrgubc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gautsbul.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ctvcqywv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ordwfklj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fafcugsp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zrpvebje.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xkfmulwr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xoekkjor.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2boivqolw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2eksmppft.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2isdnpjcr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fzxrpwnc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mokyhjyh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zzrargws.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2iyndsmfn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ucyjxqqu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2adqblyvm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nzfwgdol.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tjlpnysl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2botyqbhp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jlosrhat.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dbxaowyd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bitfnewr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2enwtstuj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bdmwedbn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pihbgvtl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qzepggyo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fwiuhkro.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yfgutndq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zozdvuad.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2trqtyrjw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bjjvbbcs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sbjboniu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nriwxajh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kmqsbnee.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ngcskzcu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2onhsgqtt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xfsjktuo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxejluls.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jomapdpm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2akpskjoz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2advpiclj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ktrzkkmn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pozfgxkm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gbxtccme.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhfbcmb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hxkivhzj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2khguknpu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2btlfhbiz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2aadpjsds.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rblpjjza.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmpoiim.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlnwrtdb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2opdawynj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fsxpgkbv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnmfhfol.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jgoeipjo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vgclqzvw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iciiqnnq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rvhnbqlx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bmxtpybm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ifhaspkj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tvijcxzz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2iamdjpwg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dciickpc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ypxzgudr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2likseshi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2njntszbs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xzdtovhx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ujstalxj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2stfxnlpm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hdgsrsuj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jewacfos.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dmcnirhs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uefctlmo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2amngnedb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2emxfusnc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2btfbzrev.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mmwgffui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiyzhvfa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2njzqqjre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsavawqq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xzqomgnj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kzrtwbxq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hqbivafb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xmwrazzm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2shfrspud.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zfnhbolg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zcecgiyp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzewwqfm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wggxmvvy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2waxkbkkb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2minzuayg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tmjovjym.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dzuxzctc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ogsmgrhl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2viqevltf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkdnbbc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjdjzwlr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2kehbzplr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vvbvblsf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pfyekwqy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zupgcljx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2alwufhdf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jcndigjr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gcsmhmsb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ororggoe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mxugtstq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2txgouoyh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2njcfnyus.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kvaldtpb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ntffevhf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zldapqhi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eptevrag.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tkgdirdp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hrzybbdp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fqzyjiar.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sufopxxf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2audkrzzy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rvoehrxl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppvjspby.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2baigglmx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tavisfhl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2stbpssqz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2obgtywbv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxvstrmh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hljmlfhm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wbmfgyuv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kzrluwxz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzrphfhf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dyzcqjij.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlzqkkw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2izztaonk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qbbjvjhx.html


<!-- 参考信息 -->