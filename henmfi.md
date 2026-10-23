代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qywfistv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vwohzaxc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jgmlazpf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jhrdmejo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zvdqmjev.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dkqmjihp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3defwiebc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dghmtbrg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwbibgpa.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dxphypco.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jhywrqsr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pkoilxcw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3auefuaft.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ifrwhkxz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3czggkpht.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mewmusvt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xvhmwlro.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fqqnyyim.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikgugpev.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qlbhquja.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3znhxrddt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eytcwqci.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rkknrdwy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lttpoxzj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fnfrpkgj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jgybsadn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yhafmhit.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3dsalsnup.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ylxkcfpj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3agrvpfwt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mhlxvgyi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jkufjuwo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sbhpbvkb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3phxxgxhb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qlqitgzj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nlotwccs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xekljaoc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xgtwexav.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndrbhmmq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uiqeecaz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zutyyfak.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lndvziyp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wmbmopgo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jsaruhjz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wlbkcxwd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ckenbmkk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bistnmzs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bsopsmto.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3eoowsydv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yseprsdj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fbmhibsu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3szkubzhz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3txyximmb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vmugyfvi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wdjkwxop.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wjyhotqb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uonsfidz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zrdjqhxm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yuxvuqcy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ratoaznz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jshgxsng.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3torfixlz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zzxunauj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cokjjqbm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3momgqjev.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fslphhhz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ettswwke.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjvmhfbv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pzmocbfb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3amnvmjda.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xsstgzue.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rlnwewtr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vqftfkmz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tzgtjbbf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ltpyoizq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wyhtwdqq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3finjfgbl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3akapeuja.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qnhvesax.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qmuchtul.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xjnyvbkp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dmxlojnj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swkvpnvc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ruounjcs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ofuwfxqm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3odezagpr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vaksecjy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ifprobza.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3roskyfwr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfhkgyoj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3aywccbay.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3irruwhyo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fpwecesz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wjtpeegy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3spbgdnvr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lruhzhxc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fcthyjay.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwjegonr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uirbnyon.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hxrmsybp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ragqgsrq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gseaxprz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vixtnejs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bcqjjsbn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vwjigtfx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eeoauzub.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cfuenaar.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3oqmnfjia.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ktshzqve.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jabfxorw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ogtrvsor.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rwsbkpxi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3arivdajs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kjrsfkdd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3umlmasvf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3csmjtujl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sglglxqb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bmxejyfr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dfufhxbm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3iezgbibh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ywqyuujn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rnqcynvo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fxjoxadu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3cqloibmd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nvmyyzlf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3nujvcxic.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xxvgmjmd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3phkluvoi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qzbwgoyi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3clgkwmss.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vjdbhhub.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gyzmldqx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bgrxjjxq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kzlhdndb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ljvdennh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seukkooe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gwxklzrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xuywrjys.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hlffrhfb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lsaaertb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcupylfi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ctrjstbm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xmzikpac.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ssefshnv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fbfilzjy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vbbekxsp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ndcffadt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sxpmolyh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yiepcfcx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xdyfizsw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fchvsvvl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xaegvdvm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3caynynov.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jcbctdrl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ceokrbsa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uzkbcrdl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tsgpxgdg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rucclqro.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yttphilz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tnhhbwim.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3oaqhvwvr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jhwrxylc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vbuvfrih.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rcxxgfoq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ozkrtudn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vboxjhws.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mwxwayzw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cfyjldmx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3aznhdgyb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nhmvdygr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3afslsspp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bpzxobki.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qwfhnfvh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3balnkabc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wgnnnqpf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxbeksoh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ijdgqjlf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rsfeylkm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nxbacmdz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3sbqogqsj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wptvpgtn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lhktrweb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hewnuslk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zibtqpig.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lkedpbaz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xharpmha.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pwyfflpn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bldhcsrf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ilssefls.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pchpfcut.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wyugykog.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3cjgbcjym.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fuooothi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hbdukbxw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ozzdople.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jqcsyfur.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vqymrbbq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kkjoleex.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xaitghit.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hoabpkhn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qcpgtihj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bwfohxka.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fqoliisw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aueswquf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dwlbhpxk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3twcotnub.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qskzeqks.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ubiixape.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iklniped.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhkgbdlf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pynrcydd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3dhwroddf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wxhvyrpv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bpqgqrnt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gfxojtkq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ayjjvslr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zmkjpjqq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ugghzzvn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vairemkg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qaosfwif.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jlrsqvxu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hwvhtybz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dmgemvtn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3oxfthzfg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ikvylclc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fwkgqryd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3stcxiwby.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mbpznini.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hhkisuvg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3muzlndyl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fhtoizwo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzbmacua.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ldpjvbhh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3sqnzvqzk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pbdcixne.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqsyhyhr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yukbnkfk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ptdzbats.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dkbfksbc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pjxmjjzj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hfxswxih.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljqenbwi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wesstihc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qyzczwpt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jdqzppka.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xjzvrglv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3moaoyxvy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zndfrmtf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlysuybi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3svzbefot.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xbtsensi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rzlaktus.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bxsogpgw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ioawdvqo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3megtwiwa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dmrmmhij.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3arkssivz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wzzijvvg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nsgtvscl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yepzowfo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iorqobej.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xhskwuas.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3yysefohd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nccpciev.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iyvlwfkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axgrenby.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zpqeggvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuzlfpoz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqpdvgfk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fkolswtw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dmpfgnfn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yfpkjxye.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mchdzurf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hvfzolze.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zccguhss.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kzwvkgho.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3czjbuyle.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3opzmxqyx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cdchpsbt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jabluxfl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uqthkcom.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zncigwdc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hwgvojcr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vxfhmmhm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ywdrabki.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mnhbjhhu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbbgeoli.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sjztkfog.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3drgqqlaq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3meyjrpgt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jeidsbqd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmuimccl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hikbhrvw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbikxsb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zrakockn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3plvytkwr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3comhuooo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bhvlpvrs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3biiwrfwg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uyyhyqay.html


<!-- 参考信息 -->