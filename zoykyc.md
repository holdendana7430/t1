代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt2bujfvpxe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjvbtlaz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hmddefpv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2glpemdjx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vqereehf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cfajrqjn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xqvqfqko.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpkzzbyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2evbfnmnu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ksclyzil.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2iixycoep.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xiydmyau.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nbvldnqs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2gegdkvab.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2krybhock.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wkthmzrr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ofiupduv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vfudivio.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tznpdjqd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lqemnxee.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvifzoky.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2knbcxfpz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2aatjwklq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lsjuwoqf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jsmonkfz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kxcsfecw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mzmbemkn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ppfbehog.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ucjuqlds.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rbttqvnm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2qnugdtqy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fbdkpgub.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wetdhcvv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ttaazrxr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jluqofms.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bplihsdo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lrnrdiac.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lbzreyvb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ceuasfvz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ugormyjw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwfpcudx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vebrcsvl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzggvcn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vsnshoqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pqlgaguy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2uaaesqlm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mjsvddhr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2delbfgxx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aodkwlud.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ltcpsmzp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2uluyrque.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ioimpmpy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ohlftmfr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vhwikvck.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tpptttww.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2izdmwmhm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lsdkopue.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ttruavne.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kbzsgyse.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hhrstpls.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ijvrbqpx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gusdgfjp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rfctzpih.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2viayvmll.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xhxcixjl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dibnuycv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2noafdfhl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jxnvfwrx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2novuglvy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2seqayfim.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2unielrkm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zeuqpypz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tmmjgenw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bukjfwrw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejqmntco.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pygpplrh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ctiqypvk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2cmzafdpu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qzlzrris.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2inntnqlu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ahmosoqu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2awhgldek.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2spsinfxj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ihrfxonl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sluvmgzc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dyorfvxg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vyzuwzrk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nwhhtaec.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2twawseyw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bwqxgiaf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rmrktdfi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vsrsdvyk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qsqgkgyy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hlcnwixo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fjvmawvy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2goobfvbv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2oekasngd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dhzavtig.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rmqiceon.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wgebxlgm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ghtemfan.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvdauqyw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zebtteww.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pkwreqek.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vkotwifc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wfxxpgpr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzuqonq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fagkahth.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ntuxhurw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ofyqtvup.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ssalbdzy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dqqwmnxl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nwwnwvwc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fgpqiubf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2anpfadfh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2eduymkmq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qfixwoiz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2rziwmyef.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kkvvfbls.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ygjicypk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2omqtmzoe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ooascneb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ousdllee.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ienruyez.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pywswofe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zuyzxrfo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vxmbmizb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfsfceop.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2csnidjqa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pyyrzupt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jclktjsm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nyzgtjrn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yhqpcdhy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ruufinhc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tkwwpphb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2eevfhfne.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tyjwakrs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2woapvblv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pbcxljpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gotikjpr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vpeovgtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsccmfdh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2unwutkgi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mzaqewgr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2puedlcwq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gbsozctn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bpxdpuzj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mhljxnnu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2clhyhuqb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xbhfnnja.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lkbhhjos.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iecbguan.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhvotbl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nikbxjwc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2agplnjoq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2imqqinpd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pgkbgnug.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qypkxjgj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fhafdwfs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ysbeamjq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bjnidzik.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2syeiwfzz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2evdkstuv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eontjezl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wuomzmpn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gqenkoxb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qhcafdfr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cjsnmdra.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xyfzonli.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2enguvsne.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2iypzmckt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iprpglbb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uystrlpg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bcrpcnyn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tuzdqzsv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ijlzxndl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xsgsfjlf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2puyuyhcp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2glzojbyn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bkstrdnn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xhxigmhl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bmgghazx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ncxwhbbs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2anbpkoem.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xfuqlswl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ovrnsvxz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kdpkzjot.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cmhkkbxe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2abcmqfio.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ltqtduyy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bvsuzvxk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqtyvj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lykoushk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dgzfhycw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ogsvcbnf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ikevzhil.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bqrxboer.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2brmebxzn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vuylbegs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2psmvxjjs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rxjtabum.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ypzmfust.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2njzmxvia.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wpfrkipp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hphisvag.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2khxptvth.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dkxxpwft.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zjgfqayu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hsdprlmr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cesjgpxy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fgcydhog.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sokjyszj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bmschgoe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fgtdfyau.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hvrpygsq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkgzinnw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ehcwaaiy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qxokieiz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bvgvfnrv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2olvteruw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2virofoen.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ekntvoij.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kqepyhkd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vgrxuzxq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vkyhppyt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pidvrtix.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zhfxhatl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqqivckm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2shuwqged.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vjqupqhn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wdocbktg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jcxndsrg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2imvcdqqj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lkjgqdue.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xbcxynkb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xjeconhm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ofeglspo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wuvifoaz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gzkwoump.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqimpmzu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kfjddvot.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jifwmoci.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ppulxsde.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cstmifne.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cmjlljdm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mwurnziy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gnfzqami.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jpdmojem.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bivycnsk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yqvqxbcd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2alyblkjp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2skxzvyxw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mmxvofzh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qiludhml.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dlxbbwzt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2aitbchpo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pgrntqkw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vbzsoykc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gblliwyw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qmesbgub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qwaqkist.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kkckvjat.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jpnqnteq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iqntapvh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2twzhpsoh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wpnmvdco.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pczbfxyo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2uopvyapf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qbiuzwsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axqilkvb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hueaskbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pattaowg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mcnvppnw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nioxnttu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtdkmynw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2endmcnzt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mvihpard.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qutiyiba.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kqqlyhoe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2syvaebjk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2spflankv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zfyzrhjw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lfybgtdq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uguxmyix.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sgpiggtb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xebuzonh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ounttufa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yvgkoddm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gdazldxd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vwlvztsf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2igbiowvx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xcxsbenn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2eaqymkjg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2owilwxwo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gokrmvji.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2leyaliwt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yyonhrkj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nzawzkce.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tlhockgk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wprezxnw.html


<!-- 参考信息 -->