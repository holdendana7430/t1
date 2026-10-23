代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt3aclkolxg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bhyjjemq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lsxofkoi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hqmdflmh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pzlteusw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3htncpylv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3enurebfu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ventjjdn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vpvhqyhw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fxxsivqm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bgrnuzar.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3irtzagnc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qcoragqy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3chbugbsm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3liixlbcl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3spntyncn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sayzubud.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ldaaltzz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bdphejmq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pwlpqlem.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3iacgoqwg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rtjkjxfz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ilhuagwk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ggzyhfir.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3cteljyop.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tpccgzcx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qwuywkqo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3elrorjvk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3mavpkcui.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3lguqayvm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cvijtkwe.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nmvntjcm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tvwblxdn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3izgrajen.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xfyrfhmx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbxesldp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhbykecd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jeoanhev.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3txnqrwoo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yeiankfp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pfcrlwkk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3honsdswm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3grrzwiro.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vckdjnyx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bchqmlwd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yajokzns.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nubdxzae.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wczjdnwi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3oojgzkxf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tglzcleq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3semtyxdi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kfpyrhhm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cifkukii.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ughbzart.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3aojpxkgp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mkzzyxro.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dnqqaelx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ghdeufwf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3uuvtppfr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lxaoubqa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zqnyifsh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dtovqxnz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xiktolee.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uyhrpbvs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yqxtupgp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3klxgndny.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lvqadsmn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nlbnmxfa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wvapnanq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pxpbqdve.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xpudncgd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zibiqbnl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sqgglysa.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oyakambu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ryyewjca.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tubfkrlt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ljhpsjeq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3arqzjrrh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lnuvbonl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3akipvhkd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3agmpmjen.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3sixgdsrv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ymoxkhpq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rxdvpnwo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jicwnnhk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oiwprsvr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwtzxzqx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qziwwalm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zaibhjcd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pumzyuvd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3demqptwc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3iglyntgu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3opxihthh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xijujxch.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pgjvvzyt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kvjzzzuc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vjkxxwca.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3plbyualw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3eeiwidir.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jxawzuhj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lhbrbusc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ydkktbch.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ocmxsghu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3invryzta.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jonazris.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3tqxpwbtz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lbnpxexf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tkmswqav.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qtqzjrqc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3spczwcri.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ichjbxho.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uqbsourv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pynsthxt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qumttgwc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rzbqohkr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tiafxrrd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vzetscau.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3iydyuldl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qrdqujqk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3usjvmlad.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ufgpkank.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3eatwoirf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvmxuset.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zvxekvok.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3yhpyxsxa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wmldqvfd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebifhwsn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3odjybwbe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ttxqyfrv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3esgzeuoa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xfxfcxbg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zmvltiqv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ttbvxxzx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3flmaeazq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tbnoeadr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ksghpcid.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3etwqkwhb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kufqqexv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3whscoicc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohywmozv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kbkoebof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnhndckd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zadovycm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3oqyyelgb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhfewzmd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hqcvbahg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cabflgmk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dguyweej.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sdhzottz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xnmhibna.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jmvhbiar.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kozqwthu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3edmxnlbw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3irmvdalq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mgdkhxpq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3uxuyiaym.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dzjfkvcg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lrjphqij.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3veqbbacn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lgfhwdvs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rztgtisb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3holqmvzh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rxdijwaf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bwelouwq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vasvnyhc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yowaovgp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sgbffuig.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bwjrdwpj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3abstalhw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wsgztrye.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mqasxjcp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3adrbahqk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3izvhndja.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rtfkmtfe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3txczfjxe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3izkxgexo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ffmgadow.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rlxvsemv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hbwmoexp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ubbwkaxh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jdizoulu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ucczltdw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bdkdvrvw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3andyldlm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3phobxwbl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3irthqslj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cyrlxuyb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3benirriz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jveizxuf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mqmioyer.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jldarefx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hsuigimc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3didvqvke.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dfwvedyc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rmygalfn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bjfxjvrr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bdnliuys.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3taklxndu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vgcbugpc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3umbttpto.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rmnphgtq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bqxoujhj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mnmkfzoa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xbqcuyqy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ylsowzir.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hwotrqem.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kdmxbqlp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dciygvfg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wiqrjbdc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3wuffyytt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3adudlwqx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rtpekidr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3uqvavkoa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3pgtohzqv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wgkwdtiz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nlcejclu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pxiuycnm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wrvyiasr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3byxhzovx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lyazdzut.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gtwfduit.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3sfskwiwd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3likrocvf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xwpkkiin.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ttoigtyg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xsikzone.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tesceqgk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oejdikdg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mjydvqqd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mmuysggt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3soqvoxfh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3evurwgdz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vgflxjgx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3egtunxow.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3orkpfmhr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gummptyg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ocruyvhj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tlcbpciz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yrzvwbxa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjoqwjog.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jvzyajxv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxzavzdr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bocurypm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cpaeogve.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bniuxpko.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ifijbyup.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3phwvagev.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vkhaxbdl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uscztmkl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3iotzbiqw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjbwjy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vjujaklr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3esvfoyqf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lwhtcexl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3buhzsvqw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3yupnmpzb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tietirlh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3utsnrbrt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pytnwykf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fgsvoblk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsxneztl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jsushdgm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3etbhmwql.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3owadevdp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zuwauaku.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qqxrqldw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gkptyknq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nmtpdvbl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yircwbod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bndbtnvd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kfoheafx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upoyteii.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tumaulkz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tyjvheyw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3sqkqwrah.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3efxlwdap.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3jtvuxenp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xremiwcu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ykkgjgpe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rnlyrute.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ekovyjpk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ccsqbbxr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3khvofrcr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fdippccs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cxuwiqea.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fuzvvado.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3arirwuvf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mwslquxd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ogrexaww.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wckygaly.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqndhtlb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dcbrbcdp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3azxspdah.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3trymzhrw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3akslrizw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qqlgjgor.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3usbywoey.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeoiryvv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3hshltvmm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3msisdnpb.html


<!-- 参考信息 -->