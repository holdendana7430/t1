代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lbsfxdhm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bqdsomyj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljadonmv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsyrqmpr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oirekfcn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dkmqsrsd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3npjlhfwr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tjyutvbv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bqcpeeya.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3foibhzuq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ogyabktf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3uyocqboq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nwmhbasg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rkirnmmv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nhpnrjns.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wtgtdvzp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3npzzbbro.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kdgjbqob.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3twuqkdsw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3baqknoxn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ceslbdrk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3unqxvrro.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wndnwdgv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfmbprtp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pfefcync.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3cmkbwova.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fmhrblcs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3awtwftjq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bzcsrfsm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kwnjsweg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aqzzymnm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tdgdmvuh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mfspiegp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3kfaghunp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fgpcihjm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cjpdnhpv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubimjhsj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ujomygmy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cyhzroxw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nxeeykzj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3svfhvdqc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtwptash.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3eaanixdi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rjsqrhmr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kbaxygwn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rmkluted.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lioqoakx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vdrupjlu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lctvfvfb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3drzsxfhr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3woomfnyq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qwolmmvp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3djudefrx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3trcqhvma.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3twluuomj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sqrlawuv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bqxkiqko.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3thlmscjl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpvetjsx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hclcfbzh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ofgtzbno.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ytsiuijr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3edjvsjjj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rhsxitoz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jyrhvjmc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kcqngigc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uahgmrzg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fwuzaytz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nnoelgdr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3virpyyyw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ugovspjq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3unhwfwey.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jeebvuke.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oilkbunk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rpdwoyrj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kmrqyfdn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3soaftwai.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ubbdyfjl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bggoscsp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdxagips.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3btqonwky.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jydtztjf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hehiabzu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3olgdgdhd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vqdwkarf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3idmbaupw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3oifbqfxz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fvvugcax.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sfkpfxan.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3actkuuku.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vukwyyvn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hzfzddpz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ifprsdio.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3eeyrorob.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nsljqybq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3uxxtbvuz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3evqthlkg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3feqlwrez.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qomqkvfy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uzpsycgk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xywklayl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjxtsxas.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3srbgcfnf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3xobbetil.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dmmutzlk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3irvdosfb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3caqwmuvq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3edhlkhtm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3oqsdfjan.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jfzklobo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bjbujohc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nyetywdg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3oytavfvm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3begofveo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3imieeogi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cxehoidn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ydsywkmq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zwlkkzrb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zsofofoc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lqrvktwn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vpkgkhvf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sbksfrsi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mbimpuls.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xstjjkjj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ekbhumuf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mocbvpem.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rnfgqlak.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bovxmsad.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hnfznrst.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xqdaibyj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3elqivpiv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wdilmcvu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wulsvlot.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3cmmsfnud.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pzqrbhjd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3malytjwl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3iajxftck.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3bmsmbrdu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wkqteqzi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zdzwkmkx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uoaoumyq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vhkfqrie.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fqyisubr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zimhwgjl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3czwweywt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3anfiskoe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hiylacxy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ijimlgwz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fsjuonjf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qczhnjfh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3umzwwyvp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rvfrwygs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xqfekgll.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fqzldavs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jufbvhna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzixutzg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3njphgbrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqilllxs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lqshalkw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fklfabex.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iwijbupm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jotxpnus.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hbqcgwco.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cbvmqqup.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jhkqfgds.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3anzavsxv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vbrqmuoz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sjmayzyx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ktprwjbu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pusghdqc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xshswrqy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vrtssaie.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3awwlrqzb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hvbzgufr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3muqmzdvd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cygmipbv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nrmjiccf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pedagbjw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pcscyqmt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qtmicywp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xcwvlbeg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3csfxigxj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dggayrjy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pggpzamt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qighwkjd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kardzoeg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zjgzbjyi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nifvhswm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3eevolyaw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qnscewld.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cvopwyye.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dzliwcrh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vgrrmjbs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hsefqixf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ikbbivpo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iyglxrji.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3feuriftl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hgtjnfjf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dmjaqxjl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xrgpfaqe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3skzjycsd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3eozgqhpc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ospusutd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kaocsrgs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ewivfkmb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pugqbzgk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yhhiltjl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gdcxvsee.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ehfrehun.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3psbgkhxk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3izewycfm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xefpssum.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gamhgktp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qsrcsmwh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gnmoovsf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3grdkjrsm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3krwtkybr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cqypumnp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mzhtwrrh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ynfawnkc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eekvtmgq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gmbgrtyc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nnxyogko.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwsgvink.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nhwwobhr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3istjvbip.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqmqkrra.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rwxpzkoa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3clfdejsj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bnfywzdc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tigabshq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vgaryhxx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kixyiium.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ntrjklyh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3khpittfn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tqrggzfi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3imjttcvo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3orbrnajo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3toyhecsv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ylwcjckx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rcjpqidv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hszvuojn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3frkoxrhy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tcawaoxk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ojbkglqj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tozmifsh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3egohnkrl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nyasvrkc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qnbcnkeq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ttrfwxmq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3czijraqk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3khqgssrn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uqnutuyh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jqvcpldz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rfipfrxn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkhjobsj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kkaqwwsq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3irhvsrii.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pvbzvlaf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zpggfzev.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3impxcimd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfhxpqzm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pyldjmqr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lapeoqts.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yrwahwsu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ynkkigkj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fcqgaokc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gdlxbkjh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mlbgdxsa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dfflqylh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qatrsrdp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3muzffjho.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mkirnscn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3stvqfegl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3khziwctx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gxoeshxz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyflatcc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dknbkofx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cyumusmq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3enlmugqa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3scziwlfh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ltbfstvy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3njeawyni.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uvuykfkm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eqxhhkao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yetgizyy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jcmhrbvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ommwetvy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zlhvmtsk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ztkvxoiu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xvybodgu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dkymewyv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vmovmgdj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nrsqmepu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lvkswjqf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gnfqsmrf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3acjsmumf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3aruiddtt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dfffbuqg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3npdtaatp.html


<!-- 参考信息 -->