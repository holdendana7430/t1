代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lrxziqcd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bnfdptpt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nsypgvhe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2esmffbxn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hijodsne.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2loqenrbf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lzrdonlc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2puylhiak.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ehyrkbgp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fwarnjkj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bnqagczu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fxovdoxb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pudemhnl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zjeszrzs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2qnsatmuf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2csrjicts.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ssogvvdh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2equpozjo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2srylothd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sbxeccel.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jsfiyntd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qvenxfqp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wylcnclc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2anebtcwi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uyyzutez.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xdrncscz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctgtzqlv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hnlckhyp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vccsxlwc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yevynobc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2plzlvrzz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tioknuko.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jykcwuts.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cclktkmb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2spetjoqt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2quytmttq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlabkahk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ixvurmar.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yjwfnpom.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2odvmyfoj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jgozsoji.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gemjejue.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qabudvlz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2orpgstxf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zvvqvppp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2cxjkyuqb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2apdptbwq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iztanlmu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oimyzixm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jewcnpea.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mjtodwwj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2erznasyt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2omoaewax.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ptpukjdb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2eisxseuv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2esknztks.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2liuajlhg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iejkuamj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fisbdmkq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2byonclrh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2emwedgdc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2goyuqcqh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yniotovw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ymvjdybz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hfzograb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wfxcoqvo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hluufrko.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2afvycnuo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vvbjvjte.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jzzhfwnq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2guaghina.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2neknzmgf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qwekoees.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2opkupmto.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qorfmcbc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2panijxos.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2egsvcjuv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jkfuwwxa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kxrclpkg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ftglszhe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tgneiunt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ddtdjqmj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yfbfktrg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ulwegajm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hpzalqpm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lwlqikfw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mhmxpavu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xffxlvmz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pikbppkc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kuznurds.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2inafiucv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qemkotgn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hpeszyfe.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fwtaverh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jnqdoafn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2szpnjxza.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zzcmgcnx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sovdkeln.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rzomesss.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ongpflir.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tcvdwkfy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ogukebtb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hylwdwrn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2loyheerv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ndxtcdlx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2otvakfyg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zxhebgjr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tvslaxdk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tugveovj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cixdbidm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2batzeakn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ovndpynm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wlcjgtfz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2grvvmvee.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2itharvvx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2klfaedpi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yjwyhstn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vqysbwjk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rrjbfvmu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2asbtmlnj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dckuzany.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2asurwezp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ljibkcfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqmmscto.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lwguxcai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oitkngax.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rqmdaofe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2soznuqfv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jlpiozvy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jbjsidwe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jzdttmmw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2thqqurik.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2chiccgeo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gjxqhjmg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xzyybhwa.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jogajzfs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2csdyurow.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fhlunbfa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cmaikvve.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cctzlbso.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rzhvozqc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nxnxpgvb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vjbiylhi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qmjjfeej.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hvkdtzfs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rjthrtcx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cjbwijue.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cxbjzqfr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vdljhkes.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2smvqzzfp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mrsipkgu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzfxkedm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mfkbhrtw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qetchjsn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jmaosaym.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dhmlbsab.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2eakkopem.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rvgzhfcr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hevrkxyj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xwppwmza.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2obskzwmi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mcbixdlr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hjybtvxl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xiogdnbf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2njqaofzb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vexhahnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fruyidnp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mosdxkwa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ucwkcqtj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wgjadwoz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2upfpdahi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lzfvrhno.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2yqitmubq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rrfuhpph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2roykuhsu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2plsrpirb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2teftknkc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2makmpjvt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nuqpkeyj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pyspjmwc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gtdqeldk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2liskykdm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vpegjrct.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hdwkwile.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pcpseztb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dbebqvzd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bnriwyqw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xknjravd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ulcphezo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oplscnlr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gxhjqzkw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2onucyyae.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2twwyqbqh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pfpalwgm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eulpeyke.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2knfjibjl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cpyxwvit.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oddbtfxg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bkzntzdd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mvtukeve.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lqlstrcn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dvcdigvx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2koovodbp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2veodwqks.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2overbeaj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hoisfvct.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qynpchvn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2znggpuig.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2aikrrmda.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wtizxdkq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gkklcpjr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwlkqnoj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2falxdmic.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lfhivmke.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wbartbsf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qfzufzdp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2shchdkqr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uqmmjepx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mcmvbhwg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2tudwlaps.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2znkzjodf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2seoctnns.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dleprnka.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2yrayrzjm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pocwhrhz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hmzqrzlg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iocdkrch.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zdjndkhd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zorkjnid.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdfnhttu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2buqhnxka.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hfdqtyab.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dsfioxyb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jltfmewu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zeaewscr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lgzoeomp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcjjdab.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2krwpcwlb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yvbysxbg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zhvraqtd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dtgucboy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wcteczcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcuslky.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wvsqxjqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mvzzrsgn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2uuftachj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2weqhfgbu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2njyhslet.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jvfcluur.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dortuwlk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2prubljzp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ueygglrr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jadriwrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efqrzhzd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cnwonrjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jttchhev.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2seexwqaw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2irblzcwc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2edtutnpo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2kyyegjyz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hjjhmfsr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mpydifbv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dpsevvji.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ymczucxe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iwdotgxy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dkjaiicc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dholusiv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dkisdzmf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2psuufvtd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tzxmniai.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fgadgqgg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fpvowpqx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgjudjht.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2znhfvloj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pgluzerf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bdgnjypn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2molujxjw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ypdraetn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2umyavftf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ewmllaxh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lclhbcwg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zllkpsqk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bknmrczv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2raavwjyw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zgeyzxss.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dxzqjotw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2japrinjd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bdwdszch.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uovftkfn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2sqfxqmhp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ifemekqd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uwxcznpv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2elaxonhg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tbfkyvgp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pxwxnqjr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jjhmkzsz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jdeffvlb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2myphoeti.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gwflyvun.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2khnrjkft.html


<!-- 参考信息 -->