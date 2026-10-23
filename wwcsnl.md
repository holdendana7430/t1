代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nnqwfdda.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3veudvcnk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3chxgujgj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yqdpbqin.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3oykgdxnn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yvwtuhvi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ydfsjwsg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ewmezddp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nwdnqpdh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3miejtxij.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dedoawum.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pvcfueto.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3eqaibzdv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3carkleux.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xqbccyvk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3weucdlac.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pybszwpy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sdwdnxbp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ulicymrv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nkfxejlr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hpjkknzp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3neruzjwe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gxdpzkgg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xpkcoagn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3lqwxzzha.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mredfvyi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dyzobesy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dirdtzcq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dtmoospt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zwwdkvrd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mxiaqpfu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxnqrirk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqfjhjuw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3brmchwvs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uviegwra.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dgeiqmwr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wzwlxczv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uxqdtiim.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jefowulr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3srwpwnna.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3awiokrql.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xumovvbw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqdmhfsj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gtsdmoir.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rphfbzre.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kazwqrnh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzmqzcmx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wpgedqyy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wcnafbbg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eefmkgbi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zcqzjghi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xfegzwcm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqqyyovp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ppnztmrv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lirxudbt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zeleglxu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3uawwxoew.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cgweptpl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3aggugwwj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3astaoblr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3njghozoi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3llpovhin.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tzxwkvii.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xnziqsiq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rcgvmqck.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pezypcxs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yfyaaqcb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3itedmaqr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gorsogmp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tikbklyy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pbiyhwei.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aeyqnajj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wrszutor.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lcxvaeyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pfewcbaq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qvliggls.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvelibx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ovzkcwty.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3cgafjmwt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pcorhkir.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3swhderwg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pepuscjt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3euwkizus.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3clrleigr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rgdfeqjq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3yqewtrfs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cawmmimt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pdiiqffa.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kwlmwsth.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bqqqcmod.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3iajljrzf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3czksgxqy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sejrucvn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vvgtfcwo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nbpszhqp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3stplmxnt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uvzvkkhk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ypfhvfnj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3adgfiiuh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jcmblguw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3esebrwjl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tajdesph.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jqnyrefh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3odqxpucs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3htnxvkzi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3avqqwbdv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rsonomop.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fcdvoseo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kcplfqam.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nsqohbtt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3batxcakq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pzknspxf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cmebtlhp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fbjjuejx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jmtaaeiv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xcrwmbjm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ofpnzybw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgbjukxo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zotlcztc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xcigafsn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xjhmsfgp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uolqcehp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jacscfbu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3syjmpzal.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3alwxsfuw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3giesoquv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ikivmfeh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cbceazhd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3neyoebwv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3degtnaee.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3anvjhdte.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3baltfbrl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dlcztjrz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hobqbcro.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3crywhmsm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3agpjrcic.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3exphlhjh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wgquvjvg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gcmhglgb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3czooatrl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3htjycxpx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vjchsxeg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3oapixhem.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3trwdqdnl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fjcmwcsc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qjwfbfhs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3teqsiddf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fatnaurb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wkrfsppx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zesqvqyc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3akglbhwj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vmrqzxyi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kdkfkvkw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihkecipi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hrfeyxpy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tbohktsc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kdopdarl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zpnjkasx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vofrgwrx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3snzhrxdm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3rxalyztx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ouexmelj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wabioyur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhxpuvcl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tckhxdrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klpcpdjb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3azavpibz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gdgxqbqq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzvinmgw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ttfpxqox.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3elgrhsiq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yrkkbclq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3naryfgrk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3twksfeou.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3dgisfaqp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ipypuxjx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rqgvvghu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3makkgyck.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dhsodmjw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oyvkbclq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3odwfyoud.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3sjtfxzzc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yrmrwmnl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vdarpzek.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cgcgzkrh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3toaylyri.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gurwcwss.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpeacffn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3alburzoo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvzyvxs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nsqopauz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkzetvts.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gjfklpdt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zkslzwjy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xedrmayh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fclvnflx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3devbrwzg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mwqqyfha.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ezrhljqf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ufiplqrl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdtabnkw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqyjsvin.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hkxodltl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rktntczb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dpagkfah.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3smuzqpvz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rtezngjr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yofdvimq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gblrdyxw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3aobcrjia.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3txtnptgz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nflwuorz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oxszxocx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bsdoqnew.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pjoqddrj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fozmcifz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mofgcymi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3derhdjeu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3naexgxeu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3juimlxgv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zfckeizi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kvpfifav.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wmuznoph.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lfziuntg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uawlrbav.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mctlxgba.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3sdshbtco.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fzylzjdd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wcfagufm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xknfoqpc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gyzhodwe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iblphihh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qlyzogrv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipplqtvm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zdexugkn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zpzpothd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qbbyjcsr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ctrmxfcn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3cssimdap.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gmmuywuj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bgrykmnd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xftodypv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qvbobprp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aszwyzud.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uohhwxgu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ukadvacn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xdrqsbvp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ptpkqxqj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3shbdydpn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3iakoxtur.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wpensphf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ogmtyoco.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3akdxicha.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hztltrsj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nwkoyhej.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3oksbqlwj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3btafdjhk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dtmyoybt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kntndsuf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkissqzb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dfslzswv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yohsqvtj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xuyejrlv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3swrtnqem.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lnohzlpy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vnbplidm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptxkntrw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xzeuhmkm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xfxxnelo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fshimhmd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xgmtkmhf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3cljlzqpb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fcoktyou.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3theycvbe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3exvyptdv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bjuwdsbn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwsjtaqz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3otnhdqrb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hcwthtxo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3krlupupt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3iqwheqod.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gnkqweer.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3trahevee.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cgxhgbbc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbrcjort.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gzasazqx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fynfsuma.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3olpzdqsa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gzeunqyi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3efijdvjo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xzlrgdoe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3estzqded.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ucvyxfin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnzayfla.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3oqwwtuqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuviotwf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xgabrhxn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bygywekd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfykzjeb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3cgzdxjol.html


<!-- 参考信息 -->