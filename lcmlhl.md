代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zgdardpy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jhiwmzke.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tzdmzntg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwdqylbs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3isebxmwc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ujbavhzh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ujoctrrw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3reqcxadx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqbnginc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xuypquwt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qswxwaek.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ijmmwunp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dgdhevqr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jniwbros.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mpkqgkpc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xmthxjua.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kbaqijit.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pbbrnbuo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvqnfxsg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3npinrvkv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mrypqdfb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bsvfixuc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3abqyopbg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ahtggemd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kgghcsub.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nsjoyuix.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wcprpzrw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bxnslcnw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rzwafgff.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kacdtcyv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qzjohymy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vszrfuzg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rfezcfwk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jvtcutbd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3abwfcuzl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3czcukief.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vddwouff.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gcpoxyoa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhidlxnv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gqpnwuiw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nejappvf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cuhveqik.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hgspfxay.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rlbuyuyf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3idmcgzic.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3efsgkbpj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qvygirvp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vklmusqz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywheszuv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3whjoiedd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gkmqrkcq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xosbgqpw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uaoungaz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dytpjses.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3oromemgr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hpgffunu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fjxkpuxe.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xuktbprk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pgcqhhfg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vjgbiwmo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sszivtxb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3wsprylht.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qhjccdbc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zmuqahub.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iiqspirp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lpgbrsfx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xxqdcjel.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zgqgeeov.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ybcmicrm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3blyictmu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lckcwrpb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rgvfhbab.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pskwuhsj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ykfcotce.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gnuidxqu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3foajjsel.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3sldpmiyk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mrajmhcu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vjeliryx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3evpxdpet.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hamojbxv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bishheln.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ubormalt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zaisrrqg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vkxapwrq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bousrtgk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bfqtabtl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3njjztlhj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wqkeuzsc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ehblppmx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bcvxgztq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fbzuzolw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3npmccjle.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pmdukmhg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dnazigfg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ojnvzffe.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qldbswwq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wmekneuz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nulzxujr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wkbmtkha.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ajgjtcea.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3abfucmob.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3aodijniz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3luxuchuk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cuaeuhbn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ambbrfpa.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bhdlgwzj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3sofnmugc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uoxypinj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kudszopv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yuwmzkzq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3eunqekdg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ytljkepw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ptghvvwp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vvaipbqk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jckpmyry.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wumtsdxr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3errppscp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3urxpscbe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yauvhwjk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3yorkgcwo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fqxxooyy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pgewaxac.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wtichhed.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zspepxtr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3luyxdbcy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tjlacrxe.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jjkkejwd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3oqnhynij.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3eauefknd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3letxofmv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tvzeyhsz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kmxgbefq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3txuilubw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ksrgzpwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icxneuzw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3aycqihwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spvxreac.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gebijuks.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xjyckopq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fvfxriqu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3odprpelr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3owlpnsrj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pyuypbeq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wqsjldeq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kmavurwv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gspefuzn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xgoiiqfz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wirntxro.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lpmdqluy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qpfpcivz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ssvtmpob.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ihdzlxgq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bfjnmjbs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3broaqzmk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3iubnbtfq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vwxvyhjg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3agyrmpge.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3unzbuody.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xenodumt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xduqzvsl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3aaxedxwp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xylcfipd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdvmwgos.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rcznzqrq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qkczfzta.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fbabbdhf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zpdokuqb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xyfktpma.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3exkkrttt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dfguzgnc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ioeiwpyx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vzltyzjg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sgwstopv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nhvwzypv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfougxhk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmhptuw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3recrspol.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fokiljif.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wyjycdbr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ptppoyaj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3sruoedpv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vldukbxf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3drgmrvna.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lvxtnzsv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wrwccizh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vmpdzbwb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xvuvyduf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gysrzxlf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rlwsoory.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rbcdaeqc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3apjplczm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dqheilpc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xiwqnzkk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3avxufjxj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ftolptyw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kpzupkut.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rbdfwcgg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tdhaasoi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ihfvfurg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3btmgihxl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mdnzijqe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ijbsufku.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vsxyjwpz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3eyrrgctk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kktwikle.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3neijqyyo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yjqnmvqr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dgjcfkbp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jiwvpkji.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wfqzkcba.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3uyhmrezs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xogxmjbg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3chykncbx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kleghnmj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pzbozzba.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3neikmxbr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3izdhjewv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tyawbqdd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qskggukz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhmjagzy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3prorkfzb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qdogmndd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ebjoqlwr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yatenawv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jackkdpd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3thsoepjg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jsfipcpy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tcugnchl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3avdpknzm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hnzgaclt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuqkrpwe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uldamsco.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qwscyuas.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3skxyakcq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jgfcatbh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3clhscspq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3uijqkrka.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fieczfjx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pjifrroo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pspkcarm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3renjkpyo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bywlworu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sbrtirff.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3husdqbtn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3exsfpsjh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fhxxkmef.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vypaabfn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vhfxdabv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cjtmxsyu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3exxaerko.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pcnwnebd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nucgizfb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pdcyhgaa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jdodzmzp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ixlbqrlz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3egcuypzt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yzgmtdaz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ymvzkbna.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nwuhgery.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ifqgfcoq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fwdzvwya.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zhxjhoxx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ygaufyko.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3unpgsckh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noqamrtz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3stqtlkeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sifdwohc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jgdhknxa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jtafeaua.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uctlgvhd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zevtugld.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zivkshyq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wyxdbnbm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mejuxypq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mpdyibxk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ositwllt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3alskgkbs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vayvkcrm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3onlejvhz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wclxsrfq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3deogupou.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3aufxwgkv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lllxujkr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3awakuqda.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wzycuyxc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ynrxlzcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yqckcorw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wslmzcej.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pabrpagn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ohvkhyjb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gauhatow.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3trmtvvcf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwrguqbq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfpktzro.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3psyorekr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eislltuo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3vebibwqw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dehjnsat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sbknfzio.html


<!-- 参考信息 -->