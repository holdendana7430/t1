代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgvopibo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tdokjdcs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3abwdjmmf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3swilnenj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zmpzjqnw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwkbckvw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vezlehns.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wotmmnmn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3prlkzgte.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bbloitjw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dmblppfg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hgswvfqb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hxfmydzu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lmxuogxh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3itybdwfp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3iwasmvgr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3aqlcfepz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3khgmafng.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zuxksjjo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sxifhipz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3alwkatqe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kewdwrkc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qataqmsm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnjeunpo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mffifxpq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ubnwqgyh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jzvilkww.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tyqrlhys.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tcjnmqwc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3iezvdgzr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pfkcvfwm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eowdyzhw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmiydjem.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hbnghwwl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vwfiiyqn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dwvcznsg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wvdmlmqg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3igkozjnc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gvkeowfr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tqvlucnk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mzoybznz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zgbaykmk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tcvkrwor.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3clloynsw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3munwubie.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3yhkfhcvt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mykjapte.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zpenusbe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dhrskspe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qofwslbb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bufzoego.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uptqqdbw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iahmgbtv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ypsrmkgz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xvicqdcu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qlbtymrc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlovzrmj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fgrahuyu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3baehkzxm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gmwevucu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3peldszwt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zquovrct.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dzudenxr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nwojhiqd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pyquvtgv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3onqfdfub.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fsysyqdx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vwyytitt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lzeasdzo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3spjosfvo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zlhmofdd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xrldexfi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3unuarpfz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nzgnfrsk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3axzybogo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qxnodxql.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3grxoptjg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hfcygpjr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gptgdumc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ssqpvlaf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vezwvkdc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3twivnmiz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ouxqtiow.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wpscyvke.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mlafsdal.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hnnkpxyc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3socoqjfu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ridoqxlz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mevmosbf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ebwxvbht.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kdnkybdw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ermrkclw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tmtsqsvy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fuycirzr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tvqrertu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvavnl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xpcguytk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xxnmqdib.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mwaqbmnz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3coabousu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fxbrztxp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fjoovorl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fwyjxesr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cniucjzb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kzsdtdsf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qywkdthg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3atmkbmyu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sabkybyw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bxkhwdhf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zekajhdh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qvduhool.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3thbievlb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3devbyfzd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hyffnarb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ehabxpfa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ecpdzmhj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cdupbitr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgnfagzt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ygwukvog.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vtapshqf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wczsgufg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3whnpxgpc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ebozfepf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3uttijqkr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bavsxxdw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3skkolagx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zpmjmtdd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nuoghcpe.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cmbvzpqi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3hinddqqa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iocxeaha.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tlacmjxd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rswzpzrg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qfoknfug.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3lindxpsj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qbubjgvs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yvrgrsif.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vcuoxixe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ejhvgwhe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3djhaneex.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rwmndtyk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3elfsqrll.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3irknbwhl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jrninjjn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dkhdyhrj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wlgzingc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fdxalitx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3szhxjqmk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hmgebdws.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rnlljiwl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nrdydiqv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3egozaciz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3yqrbhiof.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gqvbkgvh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3sszkznua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcfklxwc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wwoluhpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwxadacr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xwuvzsdv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xweoirso.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rckaczro.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3egorkkze.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3iwdgpxhv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fziyxuya.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jssemzaf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wsxbvilz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wgppuwey.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tdfvurxl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mxwzjyrp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ksbybvwr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jobhsxkr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3flzibbgi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3byxqgyed.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qzgxmmyt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pysbxmlr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nbqtteli.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rgwpjhku.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nvvjarnx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3elmtoawb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmfegyyk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wwmdhrij.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rlbzzwey.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ignpstsz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rryvrtwz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yvqovarf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nynzsuqx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3niyichco.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yofvwbzk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bucrudpy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fitqxexf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mibdfdtk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3islfqgbd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fmnjabbz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sredwyne.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cifcmvyr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kvchvcfj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3aecwnghp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3tjtlyfro.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xnkunwrx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ixsnqwuo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fxzckuwb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fvocioav.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aklppkjv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3auupdpvh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3yqvltghn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3urzyjgck.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3czasxqxh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vamrbooh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3aohqigxr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bnclyvuc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3urkxgjmp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qddmkzzp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uokywprf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3affhcyfi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3witnemjs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dxkprlhx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zllnadyo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lzpyskkr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rckhjhzz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3evquesud.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ymndpdfq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ydnoedhd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3uhqngrfq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxrrubzy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xeegojai.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xvuielgk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zmhnmfqj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jiwwotle.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cnvoywxh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zqflbsjv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rfoiozvy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3trxrxlie.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3udscqafd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3izravmfu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pypvjygm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bgrcrbqh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qngmddqy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mnylpdbz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lalpwxnc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ivkhvjjd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qirmmxrl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fmaxachk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ekyqdaoi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vygvxfgf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hlzqkmtp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pdcitprs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lzolcghl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3bjjeiqtj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hfmjtajh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qmmjtvlz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uibllhgl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fumxdcqq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ibmmpduk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vggqfnvu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tyazjdlw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eakrhrqh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svujezji.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrvjsegd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3flqvmhib.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3srcuansj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uqnahtkt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ttgwsaix.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ezaeohbc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ntjyddnc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3daalytgy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nbynnqaz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kacbmapo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jqfaaaxe.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3oenoyurh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fwpgwdeg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ahsoznkh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wlgfoaig.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ebowvdit.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nxhbbyzl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fknclafk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3poxxplnj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zwuwqgor.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3aausdnni.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pkoeocas.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vouoccws.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lxtjvvry.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3unrlbgxc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3atqfomxv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hjpcrntn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fghmjfyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lllkwhrl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tiwhuapj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdrvlgeo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hasgdauc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mqueubqk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aaobwrto.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3btjmazvh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vqysujfm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3purdihcc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qdooeskn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uiccdjwo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rvtwfgdf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gnnhfgov.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nxkmlzcg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gvqerumm.html


<!-- 参考信息 -->