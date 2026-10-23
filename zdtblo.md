代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uqksiduz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3eoefpsap.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rkefswog.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzhascve.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qpjbtvfu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kozjvoie.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ivnlklgr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tukgxcyi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rnnqtvws.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ndaisjdr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xfhlnckq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gszsqohs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gjmnacqy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rsrwgsag.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fdrfvkcr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nubbamdw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mvkjgldh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3llffuddt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ytnqtyet.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jfqfmsqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ctgeuvni.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mkghoqxb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hadactvu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ddeoouxs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kzstjipr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pjyupdpq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uxbpvbhh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bhsqvvoz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3poeuxurz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3hfrtfdpv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3icflroun.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wldxdsgh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qacjwqss.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rywchmwt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kfwthlxs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3napfrvtq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ussynpyl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sxwogwfc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiorsjpb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qugokdxq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lzpijsiu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fpvnjoaj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gwzcjera.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hkehiija.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ebeoykji.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tvvmlzdl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3smfyfvto.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vabvxlzy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ttpluofw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fcfjasar.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pdxcrdhq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3kkglsrwv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jtcvlyni.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mrrzgrus.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vvqjizhg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3mkbppebx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xhzxirru.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yskdenac.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3txqbgsnw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gdfrlnte.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3angczfds.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3javbkqbn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cizfehvz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mxqedtoj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rqhocpql.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mtthvvmk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zzxvukpf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3sezomjfy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckfjerzt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3crodgbye.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dprbecns.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3lzbdazfj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ceccdvab.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rnxnfnqc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dkjhhtgm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3slvnieqa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ufebqfts.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rjycpqqv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vdkraqxg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lgjhfbhx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dyticrex.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3lpwvqbzo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hdmcobjp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hxflrrkv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3oumvaien.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uuawhrbh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kizxnncd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3cfwpvhwb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ixdtydoo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xoecqsfe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yyinbkor.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3glsjmuzc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rlzhucyp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qvxyuomz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jcgycxev.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jjfxjvch.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3idrdnuxt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hjtngzar.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nfsoavwj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wzkkppiv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ahybxkls.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mlkgyejq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3idfjkxqx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3parzxesr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wahdzcev.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zyvvsncy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bkzbnotl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rlczqrxz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qarxgazh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3iuzbtzzf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zroqodbg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3giqvzaen.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zeltkjoq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kyqtfdci.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3whvxzkrl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mgllqkcz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xjvstauh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qaccbqwe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qtkmppum.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sslioxfc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3sssqhots.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3avqlwfwb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zzxcfkmy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3irklyiww.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zhigupmt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqlmhgqq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jcdwjphp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rpkqvlho.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3idjuffsu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3izeaqhsu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gzdtxwvo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sgcbxvkt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gsbqnkfq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vmniodva.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ksemdkbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3faesfhrn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rndjmqug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npevlnyw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rwnevucw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wiaykzab.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wawevmlg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qcmkkazi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qtxirdec.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3juvwktnp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pynflqii.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3byodyqcn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3enfeyvqm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eyclfqel.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztimazcz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fmrtirbk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3acxaiaen.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yfeuqyhd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hvgpvfyf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ymfhjnwa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vedhqrja.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kitbismb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qtearaxr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qcgjnkib.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sohxzpwi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hugafwvd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qhemaezl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3agggorus.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wougiuku.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lfqdofwq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3amuovjok.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3boutfxnp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ygjshqyq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bpydxppn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qdfxorpy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qisebfzs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3isswjktd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tphabddi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgohtpwe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mwfnaguh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3skzmfwuc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fkjqlekc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rmtsomlb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ntqjbvaa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ztdtmvbu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vkkbgzam.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ixcgmftm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3eoddleyu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3omimgqbt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jtsdmhgb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wqkxbbpr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mgbxclls.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cmlfxsno.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ntnjjgmk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rzizpkim.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fxnlalfy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kuamonqd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hqyfsxwk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kvushysn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dglilzjt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3geuockok.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gumoewhy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mphmrbxu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxjrnwzq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dinfzhpg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ldslubds.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3suxmxtjt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pffpvqco.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xqltmxfi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kbbzkzfm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xzukyvnx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cvagacbi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuaobtsj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pzobjraz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fsrktybq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lsfyehom.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kouvtmrb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ryurpoiq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tekraakc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sbsrpwar.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zffsioee.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3luprnyzq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3femwzyxa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tdlabbbq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3aninjdnh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rflxpiqx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dqowykym.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3offyovev.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ndrsheoq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wwdlnvrr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kefnerbw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rwsjhrlp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vufviugq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ojtqajvd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mpyqhfks.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bpqgprvv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xuldwzoo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lymnqmdf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3azjxmwkb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zvmpvevg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uqwtwyht.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dtybeppr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qjelcyvl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hdjnylqq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsbrgtld.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3upzgftfg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mfhiozmo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3stdlruiq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cktvhioq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3svobcywn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yeburhhu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bzrkkebu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sygaurvo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3issndbhf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdycypua.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fxlokuhn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zfmoyava.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fyxnlmgt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nofawhyu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3guakxlux.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lbwscqrm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lqxjwttf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixplubva.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3eymxsfka.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3csgtelpk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xbgylxwf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3srntarrg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hfsoithh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3scqcvxmp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fnskvvrl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3quceztsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjgivldw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jnmdpaac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqizqjri.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3potvunbt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yhvpbxpm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdevfpmk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3akwrtuiu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dngtyrbm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jaetfxux.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xhknypsr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vvmcwuqp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cohpeoyq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3helbvwgk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kodkhqnl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zvsgueqt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qljuajzx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mamylytp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iodoxmej.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iicwpqld.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3evicgeal.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kilswjmp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zbrjvete.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jqnrykwp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pdggpbnv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tyinvtje.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xsiivkfc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xbojunda.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dvxmhhhe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3istqbcmc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zdbdpatg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3obsmgfsf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uibohwhr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdeoeto.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yyxvbffd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iwezgyeg.html


<!-- 参考信息 -->