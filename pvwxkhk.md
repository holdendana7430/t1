代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gpzntvjfk.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/ghulbmisn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfprcaxlw.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gzobrqowb.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/guatqrsdj.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gfxabmade.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gpintdmql.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gmlkbmepp.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gwoooblga.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gswpdqtcm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gfcwyasts.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gmsisclbm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/guopgypvb.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gmdlzorkp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnvmdrcef.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmlqdrohg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gfylyecez.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gogkjewjh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gtwxauoaz.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/ghtskckfu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gieoictnl.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/ggotukquc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/ggaaatzfl.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/glxhmfbib.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gwmpcmxkh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gmlpclcah.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gwgmqblir.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gwwzqpdnu.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gubbwhkwr.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gaxgcluqv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdpllmrdm.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gtfjqnmyb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/glqvvfxla.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ghjebdiwz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gccfrcpwi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gfqisyvec.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gzrihgibb.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gsyhrokcm.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/ganvmxipu.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gtriadeys.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/ggyrpnsww.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gyajpjema.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/ggiqbqrei.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gvvuswmte.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gfzzpyvnb.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gfycpcmqu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gnpbqozhl.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gwnadtocm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gjsrdwwhn.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gyddzqaki.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gaeafpuka.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gvjgsgbin.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gardkrvog.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gldcwafwv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gazwqhgsr.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gsjvrrtqv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gewegozom.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gmfuhrinh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gyvajtktp.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gfsvmffcr.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gbxsiwtry.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gjnloglgo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gyochkivx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gdeijecxu.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gjiyxtzcp.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/ggccdcnvi.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gahrnluft.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gchxpweqs.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gkofmmlxk.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gahbyudqz.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxkalvfjp.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/giazhncdg.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gfsscmlbi.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gqvjrtqfb.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gecnyjkwa.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/ggtypektu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gseuzccdx.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/ggjsklicu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gxmxcfjfh.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gptpiogep.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gafhplryp.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gxnnzkqmg.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/glpmodsjr.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gxeozvjns.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gambswntg.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gsiehuoba.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmveytcwv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/grdkkkviz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gmlxkcomt.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gxhijczlz.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkeotnojo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gppcqyvib.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gfgrybqht.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gglaskxpt.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtiropniw.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gsfsytjfj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/guhcbdwtr.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/glumaolam.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gkdagfdgs.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/grqjtbevu.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gismqzfdh.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gnkyzrwfo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gckkjbkiq.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/goxbijfqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gkspccrxp.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gwnycpwgu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gizfcuayi.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gpwqzerdy.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gjgeqspzd.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gdbqytgrk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/guorlxjni.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gwpdsgsfv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/ghcnqkzil.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/glwxttcng.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gwdahgoka.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/goodakznr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/glmishmsj.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/ghpoyxbcw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gysoiykks.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gvibkfemx.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/ghssqdjsv.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gtlmugubp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdifyrvgt.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gutphjqmq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gguvzsfco.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/grswejrhc.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gptwnhvlm.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gzrldpgqh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gkrflladg.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gzjdseuvt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnbkaqoot.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gnivumeay.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gthsixloy.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gddnnrpfp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gtcrcjcii.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gxuwjfugd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gqxiihfwi.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gxccyrigl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gazlnlzno.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gslyjxves.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gtitebnyf.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gqtuzetma.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/ggkrkwsum.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gpvqvehbh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gvsrdcabk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gjyomtemi.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/ghocjqnkw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpxwyqcsb.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gpazkkvio.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqvdhsart.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gaxfzwlae.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gporfbnfr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/glbrmpfst.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gtqhorjna.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gopvyhxce.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gkcesxlof.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/guwtoresr.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/ghyzcexst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbtymoicy.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gjewotlvw.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gfctsxolx.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/grctldenu.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gbuxxtgem.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gbfiesuep.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/ghjuhdpzi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/giufslopk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gaaucgmcc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gperjihnn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gdaluujzt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/guzhcvrwa.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gfayjrsch.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gsfinepij.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gsgohxdiv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gzxxujsfx.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gpieuxxgb.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gxsygpbay.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gbwdmwamk.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gkleajrip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/ggzzfixuj.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gzqwalodp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gdewspqkc.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/givxsqjdp.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gxtbpyxzn.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/glpsesxsq.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gjoupekqz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gnqgzukkr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gnyttnjbc.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gkzbecxhm.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/guolxvekc.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/glwznosnz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gfosecylw.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/ggtvzdksj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfihjgzeg.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gmqndeush.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gluunarcr.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gqyklagou.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gngvigzvb.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gxxnbyqwz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gqfgpptka.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gxskcxwpt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gvwgslyfa.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gvwabvoss.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gljqfivfk.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gusqitner.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gnixrqawn.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/grvwtpwvf.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gchlwneuf.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gizmapxgm.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gufwnrbqi.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gpsjysqyu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ghqwfiaya.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gzcjwyvqe.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gmmkenkpe.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gbvmyzqpt.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gaocltyty.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghzmtzjjr.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gssxwdbse.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/ghnozspzz.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gftieroca.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gtitqhlsd.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gcdvpakju.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gkwhzpgfh.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/glltrrpvn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gaamgfvfx.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gxlexzlsb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gsbsnbihu.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gfbzvxzki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gvdzmefzk.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gwwacxsag.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/ghsxzxprs.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/ggjqbjbzj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gmwfxrlra.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gppmfryzj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gjppsmgne.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gtbzsccdo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gqqawbuiu.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gxgioupli.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gxglyanpa.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/ghezcxmtn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gdvjklpbs.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gzjdukdpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gcvgiavov.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gfzswyyns.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gvibaatfx.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gbdfrbjoo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gtobhmtos.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gacwznrda.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gffyymkhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gqpysdxlk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdykktln.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gisuutltl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gfcdbjnvj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gkdqexzhm.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gbxvsftqu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gkszhtsyz.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gxmptrswj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxyjzekhg.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gaugxyqlz.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/giqesghiu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gqvjpngtn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gkoxcanhm.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gdttbkrgr.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gpouudtyz.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gxofsscuy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gjwgzalkh.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gucnkbjgs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gpuqyfskk.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gavvenghq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gczfmbwuw.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/geglblpra.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gnuposxpt.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gvsexwikg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gkkihoixj.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gxvalorcf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gonwaxgdv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gkpikuhle.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gxixuxvlk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gltkfmgvy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gwcqvzurr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnyjoonfd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcphrpmun.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gnjhxpqfa.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/giantgrqx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gbxdklszx.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gnakffsol.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gvicmsblu.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gcfgaafbm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/guhykjdxa.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gwdgtfaeu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gxxvjxxvi.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gzvhjziky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsptarhsa.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gfkrkqfim.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gmaefzznw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gdgetnjva.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gwrfsqzbr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gfbcjlclk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gwoqzdysd.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gbdcfeqnk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gjrpcraiz.sHtML


<!-- 参考信息 -->