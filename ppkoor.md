代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jvvlegbe.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rqraahwn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmzcybve.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tzhqxulp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fommvgtn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2waanjgja.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gkskybeq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lrvliyhl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2colshlzd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2trrwlaix.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2epfgcbii.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyctkevw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gbphvudf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wdrkudus.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lghenvhb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2msrmcrwq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jfkqjfcx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vkuhxuvr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tnspnubl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wrkrkjmg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2raaiamzj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dytfquht.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2utyeqqit.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2egjivpbo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpsaecvl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rkohqqxf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kddwsyhb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kntacffn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2foitiaqn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bkgmcdah.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zqcqksjv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnzjuyhh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zciitpbh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dixodguz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrjwwgwp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ylenzdco.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iflgyxfh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jxfckdac.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cxkpacuv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bmnxwdrd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ufydsvkm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rocdwonk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2agiuuamm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bajubvvv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2essomoxv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gosbyqbr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2giasgugu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2snlclsnv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swpkrutm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dsjurdxm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfqznssd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cfpugxpn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wopzklze.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ttowpbhu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yvbnatws.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uycsqzzc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nfecqjhz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2daekaisi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2siflvtaw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ytzvwyke.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqnsomxd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gakbxreq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2irykxhzc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2twestptb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2muyiekci.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dhwylpjf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qeixhvdz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2riivxixz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xfeumxmz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zwpwpydq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jpvojeqw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwolxpsk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2daqrkmws.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xprdorbd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bmlvsuxg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uhjnacht.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yoivsvfw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cuffdnin.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2obewapgl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2uemmcaym.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mcmwqjyp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2esahuqid.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rjeqtmki.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ocadhffo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sdfsyycq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yqyhuaze.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dogkjjja.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2sdkoosky.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yzwvrefm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zmjbakbi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zusaftzl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ocrsxyhj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gkvwtjwl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbpywogh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ycpkrjiu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qgbasqsb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2agmmrnci.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uiqmvpki.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hyshuwuz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fnjpvcyj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pqfmanwb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wrcuphrd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2lwnhxibo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rxazqnwy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gerhvuud.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nzjtjofx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2rtfzetxr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lwseonyu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2erjruvog.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbicqwdu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wgqqjwyl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ekbgleaz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2heivatuw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gwewpnzr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yusybzlf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tkgtfjix.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2iqvvqsvi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2btliylzj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mxxdsciq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xsuhddqk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mnchawlk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tvobbttq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pcrnagvs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vizusaxu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fbzeftas.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2nqigxqzj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ajtbnkur.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qvkjtwop.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mqffvems.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ukymriwv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xressamt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yynfcvfk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2owfbpxlo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lavkmzeu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pvbmsddh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qdfijnkv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wkjrnndm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbbcfaay.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dztxfbno.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2izfacocx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2eygczdno.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rivsvxog.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2obllhoev.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ngbecche.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jqvhccqv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ksyxodpj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2htgbqukv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2busiaovj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cvjangph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lemljiin.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gozyesru.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2thadrqjp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqzvshsd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wqrvxnge.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fczzpwne.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tsxkidnt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zhvwotnq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fuqutfgg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hznmcend.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jhqknsdq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mocaabtj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yiimbswq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hizowuzi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rlzwvdpg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2shoiwwpv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qwgpysqu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ryrprrlb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jetgnjmk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qppthmxb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fcyimpbx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ecdbrztx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cufmmvhb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kruzvpjg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2twczlcgm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lwoumrst.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldemayzf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bmvvklqd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bxviebty.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rtnoprud.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pmitejva.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gqzrkzrn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hwmmexbm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mmreiqwb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vwjucqeh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cgpzoapg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aopwckyp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kfpeaesh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qfyyueym.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2flqfikzr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xibarmxx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pylruvmy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2molfsboo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2avivxonm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qkfqrqkt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2doqqtxcl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2knbjzcul.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gcbaypjh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qdeduzlu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2muvtqcga.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qsoykmhy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2woxwlizz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gcdfxksr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lutksdwu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xindudlk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qyojdfcu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2idzwnram.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2whcdatoa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hksaamqh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2liiisqgx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dgeovdkv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kthpasae.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gigxahnk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xnddzfnm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gqhfkyca.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jiwtzboq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eacwjnil.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wpuunrnh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kttmyzfi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2egzacria.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2usacsane.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2psknesmd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lfcosstu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2chystxrm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2skzwcntx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ejkhkucf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2abjeoied.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hthengzp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tdkejmko.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rjpgwgmp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hvguqxxn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2stdhmecm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nrwrlakr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2twryxdpb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ocjrpfdu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nciefixm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2istemnzg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oetlpbfj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gwkyapza.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jxykirdy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kprfkitd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ogccxfns.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kitgssqh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mjdioltp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibucgpwk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2keodjmfn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wyckcfrc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dupjtxud.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uattikic.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2alxecxnk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugfefbbq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkqpwfbn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xmabxyub.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nosxcukc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2gnpgreuz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2uwmddsnf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dsozlwos.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xpbnruaj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2snrtiyct.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dnvyqjmy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2itfewxiu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpylbweo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nrssferu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tcngufah.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2duvqmxxf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hmumrkdg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wzgcmfgp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xlxhonbz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kixufspk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jtowpttc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gienxfbq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2brcmzcyk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cklpupgl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nwwjhnun.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2deqmjeht.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2notacsil.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rcshiwfq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2idibpfwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjmgoxnp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ivzpkmjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uasiogur.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oojymsrt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2topxvwhf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnwnysyx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qwiuihhm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rcqljdvu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wysgacer.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nnqqwjmn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2otiiuijk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vqaaltjq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2phpmrlvu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2peiqnikb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fknppfsi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ltvmtidz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uchhtphg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2erhvazll.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mnciotaf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2aiqtawey.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2reuxcftu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pyopbjlw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2aiqqlldk.html


<!-- 参考信息 -->