代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vnujtzmq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hmucteje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3osmpqrcn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3swotblxp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dgnwezii.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tntxxqbm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nnhpwpar.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rubcjngk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3subhpvyw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mnabmyxo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3juhiahqc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rhmyvikd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3csfepsrt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wuhdyucm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wtfwimat.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mlktjvtc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sqkomwmq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wdbftmml.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecyxqkct.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wiqtpeaa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3onceclzh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3idflddho.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uoebznmq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bqnamixz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxjgqfcl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bdwpofam.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3flyzaddp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rackxkgn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ktfjwyij.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3auqayxxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gcgtubds.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hudzwhyr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3azoxyiwv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rkbujppz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3wozoyroo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rgfrvuzl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3izsimube.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nyliqxxk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rybdfqsb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xyqrurbc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmptjrsj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qlgtjbjt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qupcujtv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3audidmas.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fmjddnif.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fsbzorkx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3apjvyyby.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgwjcidj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmphcccq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dniclnly.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3msmfkfip.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3etkdkoad.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3sqznuees.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cikrhdpe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbfqloft.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tkhnlbdk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zguaakos.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ltqefngd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gxhojtpd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lzgcrmnw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ssragytq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ansmhvzg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3knmekkce.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gxpmdozq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iszruhuc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3htwxzkni.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fqldtknn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lxgssezn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3adlbanns.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mcqxemfs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ibmmoczy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3iyvaxepb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rdtanekk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jnjokrpe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3skovyxar.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dmxqaemf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3iyxjrvyx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ckeklghy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mdqllhdx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hgbqblxy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yqbpewxf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fkdjofsu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ijiinwzv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3izbizfel.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3azgepgfg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bctwyklv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qiydsfli.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zwedndwa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jrvvdqlw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sjvkpydq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dbonadow.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zankzdru.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dlptilgg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dvxyinsa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymbrwvrm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yjjrgjtq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3khfzoydb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3baetfvus.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3gmmnpgjl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3svqgyhve.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3txnvtzhg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lqfrmlxg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cfucejjk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3azofbtzl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ecwbpbva.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3srtywfln.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3kqavqyjp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ofyoxjyb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fyjoymti.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yvjougwu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3azufzlsa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3gacdqdmp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uojsqiqe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvhaozpg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kvwxfhoo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nwdnxfqz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pgfppaiu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3uvzmijwi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zejydzys.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3iatcusxm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3izcpvgia.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qxkqhexo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ungpwhqe.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fhbhovxj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mghucspq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ehwfgpzt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wuxenkmq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qvfsgxfa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yywicqbt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rfrmarfv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3dudcoyla.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vysokkez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jmjlzupp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gqckjxub.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rzufwhrn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jsnsfdmj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bddptmsa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3bvlpvzre.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dkoaoxav.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3emzrlwwe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gfpbyoom.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mhgimrgd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vimgpiky.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jeasodvv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gshnpfao.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ltvpstfx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qmlrjttm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nulksgnw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fdmzauis.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vyxgatju.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mdjxgewk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhoqymqb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fdfujuef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hazkkyjh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wfaziiex.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cnvubrnh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gwgjfawd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cqdclose.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3gukmlbuz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lqlyybjd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sskcajzx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3baalbupu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3oobqbiuk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lawvwtbc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hmwnerpg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gjbqydob.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xmclrluf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yemourwe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3uiwxahlv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wwbagbvg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lcqcvfgi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vetapvyi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cnrqbije.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ydncdker.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cteruwdo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cktjvdxd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3eisnqiaq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wcuowmkw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xkixruzd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xuraywpa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xfrbicyy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mrgqibcm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tatrtcdb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3muwfiqpp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tvzlwcxm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qksjbbik.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wxsvosjr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xbzahkuo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zuafiuef.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3phlfwvdg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3pcjxnrdb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aztnluqf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3czmluumj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ihpawpul.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zliqeqnh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vhkpnsab.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wjbkzdgw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gbimqayj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3javdaeke.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ewcudgix.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ncxmuthl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jloezero.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3icqedjcj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hkgsygte.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pydrcugr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gagnjtqz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rfzrzwji.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3iwtynxzb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vejhwaru.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bpigkgny.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gamtzovp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3irogjhzg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3geqwooyc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ietgkvmc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lojbmqqw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qpbqadkd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nftkbwig.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3abyoevai.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ciglpoon.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lzlyavsn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3usshwpiw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfiwmqiq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3flltnzzu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hapgqovm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lbgdjlci.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kduktnls.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3snxdeedb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3grvaqjje.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3njhttgyf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bnqjbhaa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lgmqmute.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kxadsizd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ouubzqsg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3aguocwmk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ftwyxxqh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rlsrspge.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3uygojisi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zkldvgxw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ylpkxubv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yppgudel.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhhnmqea.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mdmjzcmi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3thmueeyq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jdghhogp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xgllppfr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ylhegpvf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hpdorpzu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vwzanelw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3djvgdzlp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xnrsdyif.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3czmwcxvk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xyatpyas.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dthyjmie.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3suzgxuts.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3idhhbsmk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3cgnkgxuk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jfrkcwfk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrrlnkzd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qkakxkzs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gdvgqnsp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pytoxugh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ttfrhwgi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dwtzgfuf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bscdofxi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltfvatdt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hqbwdbjn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hfrsihiz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hkhvewrg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qfgbonhv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3auedhmhe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pspfnleg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lqzetcid.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cccuvpbk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3okibvchr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vkesxyjt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3snzhivmo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ygrxxvxm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nrpyhhvm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3nebnwncw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ionminfn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jhbmfokg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vihicdyj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rurggjak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuynyisl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cixwyitb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3shdkllfe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3pyfkcifh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fazjkphk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3penysfuc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uyffzjyt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ugjpfjgf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yuhxjsny.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rrhiqpdf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qbdogjsg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nrctzndl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3knuswvpo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3exwoblus.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3aqbxqeti.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jgpyteoz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aqmwwpui.html


<!-- 参考信息 -->