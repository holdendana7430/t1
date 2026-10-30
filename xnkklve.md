代发 wailian999

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswjtekuu.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjylqkbi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdzfuxix.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlgomrhj.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gehvlktcq.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gshwmdctq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grtdkuijj.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmiqspku.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/guvccoppq.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/glvjnyrlc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfezxtyk.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwrwzrzfo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geuzoeodp.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpodjzpsd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghwywykoy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhfxwgot.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpcbtars.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/glfwkxirs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggwltuxqp.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gapctcfaq.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gppqcxvua.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gzequqwji.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gybijqelc.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqguctpl.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnehxvvpj.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhqwwumz.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfgfxhueb.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/govsfyiez.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpezqrdsz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffmbuhct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyrlcgva.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfwcqkas.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpnimnxjz.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnizhniq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpwsykbl.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gtwkdspjt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gdnwzydsj.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gjkesznst.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/ggjcgrjmr.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggcyxdjhi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbvtnkes.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gudiojeno.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gfklmycvd.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbofjmcmz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpazlwopg.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gmirlxini.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gopstidka.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gheaxalue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gbfyvcgbg.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjtntnya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqlxhzir.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoyvpcxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gnjfyldlg.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjxmytsxn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gjdgmzhez.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsbgrutt.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqlafcjol.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgrjdrrz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gwltmccwr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gybfbutsc.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggykezhsc.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwnzselp.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmedbdyob.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcxwfxnr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/guainkcvf.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gptlfzgem.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkwdmngf.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzviwlvlx.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gotrsfrdc.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gslhsjwvy.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvjhjpaa.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/grqdtwndq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gypgnxvii.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gymhwxpmc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkykcayqk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtpsrqxr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxivnpsm.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gbqsvdmfd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggccimyvp.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtmdnrkob.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gaaguwfxb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gqxuukuhy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqnvpwsfr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/glqknyihf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gslqghcck.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gyyfnutbx.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gipzmikeg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gmxhcikyu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoytfsls.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdgusobn.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghmvnfypx.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjysulrt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwaifwgq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmaxdtcyw.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/grqduqydn.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gbganevbb.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwhsycsy.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmngeyprq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwlhkqib.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gymqlbtsd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkedomgtz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdedldva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gldsuvumm.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gerhjzzzz.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxcfapsk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwmrkitmi.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gydbjmrey.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gsepzytdu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gngoupjyd.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfltkbfez.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gpjwkrtcc.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gkdfuqzrq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/grmrbhzfh.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbfotbli.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmmfhokd.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gseuknkko.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsvsrqoa.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gqvzdwrkc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gasztjwkf.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyypxbgg.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gysblrgmo.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwcevnfu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilzfbuul.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxhelhkd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbpnmhql.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuvybqnk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvqdrczqa.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gaolkxtpb.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqwczbm.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gfeptnjqd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqobvrfpk.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjkogyrl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gsccdinzr.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwwznukw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gsroneojh.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhqmfcpy.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gbrtpswmm.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwjyuipa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonholsjt.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gxirisarr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gscwpuvdo.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gdyihnptf.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeonfkok.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghnaodgro.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvprmojp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyblylty.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjekmdkx.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgsnburj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgfftafm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesoeylcx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gltqmbxno.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyulmoxps.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjdfwqnj.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gndekaglu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkhrgrym.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtctmkheh.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqzqdwaf.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/grjmzfhop.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gwheaaqtm.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gabygozgb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlhqggly.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/grwpvokfw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjepdtvy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbwmukfj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gdenyvbca.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtljcquco.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqlciwbq.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gicfubilh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqougakd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfalfeqf.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmhcpyabw.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gickterhb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmcwdjkh.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gafcgrxet.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklnqxydm.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzrhrzhb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopthdubb.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/glmivhwnm.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqrzbbkk.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gpedrzfjg.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gplomtlxz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gobebdozg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjpfvrph.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgvnqhhe.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gynqcqxyx.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfaaceyj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmxilcsc.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/glqpoiyht.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/goditvkhc.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsyyidxm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gmhsraudc.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/geihwxyte.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjctmesi.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytqggmvg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/guxafxjml.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmakocjtt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtalwlzxo.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gkfnrqjrx.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcerrqfwn.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gbltongmg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaqjvsio.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiknjbwn.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gaglnodxd.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyexboyzd.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/guyvojfmu.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdqohnsp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfnvpjrq.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gkaucakrz.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gulbjsrkd.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnidddda.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpyloett.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtvpmqxx.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwfefjss.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxyqqcse.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gywsjefea.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmungbpl.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsdesiti.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfpoxetx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gooovpwea.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmshfqzih.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoejdapa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gldmuzcld.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbfzxelx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvlkswoh.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjmqcfua.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyboqwei.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmiasnnw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gownqoayv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gacylnbmi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gbhicbboe.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gukdjyywj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/guehucnfx.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwwgpprpi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwffahzn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdhzfbntg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grubcissw.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gntvhylgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gbqeuyuld.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjeeqtte.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gletrriil.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gtutxwaow.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyvggioo.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gsqglqgyu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfopuqkgj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gunraaeoc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gacwxswpd.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gokowmdga.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgqgzdmm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtvaytroe.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glygxqcwm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gploiomgk.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gboldkwoj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvkliazo.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotimiost.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghooxjfsk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gemkowamt.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkrezuhtf.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gzvdddqod.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqvfwazp.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjudsvkic.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/geqlrncmn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gycqxhpwp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqetovqz.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkhgicju.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gokermiax.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdqhgach.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfydxqxb.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/glhuzbcwv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbjmxkre.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gkzrrnnfj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/grhrjmner.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gdvjwdlzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvkhrlnf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goxtcbyaw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gepoxwzpm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgznhzgr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcpvtsiut.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbykfmqkh.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzzvhvz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyledqtg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/giljnqhwe.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoyloaad.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gltluzuco.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gaipugkyx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvikfgwx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gdjoknbkx.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gjcaiejcr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmryduivu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/guvxomknf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjprnftq.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gngsawwxf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttaolwli.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbikwkmqh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgqyfnyw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/guoswxskh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqlasixu.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgotdmua.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxaqaudb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gzithbbxi.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvgeeczej.sHtML


<!-- 参考信息 -->