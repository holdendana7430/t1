代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghwtggajo.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/ghsycybfb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpygtkiz.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjtyeous.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfaiilfax.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqsnzwq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvvyihvk.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gocnzadmo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/geawxpbgl.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdvimcoy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvqtfqda.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/guyfotokp.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnmqyzqw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpnslday.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzpacomh.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcksngov.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gddfrbene.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gqzechrtk.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnxzoogu.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxfzqwtwp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavzrhzjo.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqbozqizd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonamozkb.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gjnvmejzu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsnjqiov.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggosphclu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdkyzyhd.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gxflqkqrx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/grhfavwbf.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptrqxgxr.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/goleflwob.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guewrdqwz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghigtbvpa.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitsjlpli.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjodfhocn.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjqakzmk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gszaruiqt.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gffkucurb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcijuapag.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gxmgrovvo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmqawpik.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gnheccqqt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuwuaayq.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gmswwwvng.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokjikpcw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywapdsxe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcptdfpmp.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmimhkbeq.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmyoyfuc.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gsljxrslq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrbvlvze.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/grvdslpgg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifxvioib.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufuampxa.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkocfyus.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gstbzibop.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwywudkm.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gkuhfqefd.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmrraoycl.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpntkoqzc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjqscinv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlipjwhs.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfatjcrgh.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbebuhvee.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmugkpezx.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/geyaomnww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/genitojzh.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgdkeecj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxgaheda.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gxkqodpat.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtolduyst.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfrtsywh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gfeewbsgv.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekfosdrl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxntltfv.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/ghnwprxgu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/glkahkqgi.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmfeectm.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqjtlkdok.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhnwurno.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glwpllrxf.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwuwxsca.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnstugsby.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/glfxyvqbe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyvaullu.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipyswliy.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/ganpvogor.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdhmneng.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gztzhlvmb.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gugsxipbz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gpcqkxrua.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmiukxve.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdsmjppn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbhpkey.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzfnyvca.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrdvwqvu.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gnfcevoft.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxbojesi.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gtqmbzqrm.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gelvxprgb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmnsnnzc.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfisqjcr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgavmdun.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzydxiuq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gxmdppcsl.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gnwehdpfz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwyehjxu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqgqtylj.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gtroxozqs.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzuprhsk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnicywamu.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gnittbydt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gjiddxukd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/giletmwqr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/guoeqrblh.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gatpwuvkz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gkovvfgdc.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/ghmoirqgb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwepkrktn.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsalzniea.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gchzvbndo.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdlnyuot.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqkrewlm.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gucmudvpu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gdxbzehdx.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goqxivzch.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdajwxcz.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gvweojtyd.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gezthgqch.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gkedafuhf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glpyluknb.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gqgruhqfb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grfvhvems.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ghbutqtpg.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfahgboys.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzurfqlxg.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gsasqcqva.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywzsylvm.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gexcjfwvi.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/girigoxew.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwaqrcwal.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gmizwkkgh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgadhmqi.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gstuaaozb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnjyslre.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gfipvkvme.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gndeeudfi.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjybjynr.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhznxifc.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqlsffktr.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxwspyd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatvwvyel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmaymlwv.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcptawqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/goxcnleco.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gaostvfyf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjwzxwkh.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gbtvpyscf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gonnrrohf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijqmzhsp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/garvfvbzj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gkzwcqhdw.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gcolgtxhg.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkrgfmqr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbzctua.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gprfjkkod.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiwugtiy.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ggwcwsysu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gipvlhvvg.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghoemhfwh.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglcestxv.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbrqgjec.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfwkoox.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gyebznbyx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gbuzxrsxq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnjjrgzf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzitefef.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnpptihvk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegakkrto.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gyfywwddb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ggdrqlzlv.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvgfhvdi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjlzyrmn.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcoxxayk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gzajkygzl.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/glahdksgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gmqzpwelq.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gciqfyufg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/glsohcatn.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/glrftpzic.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyuqqkcs.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/glgluonlm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjblzottw.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpytnxybs.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqyqrbmg.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnqnxmck.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchpllzvp.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmodiimhz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebftuqtn.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gkecuoktr.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqhhvzfy.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldqpsgqh.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gjxfdcczq.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqjrzdfnc.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjlyecay.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfknzegrv.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnvvbdem.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuzxursm.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdvdgzha.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gjutqaodt.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gjqvodvrf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeeqiarw.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgegpqdi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjpjjnqtk.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gzqsqmwpb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbpbbklw.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gxotsscrt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/griabmgmr.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/goazsvkzf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gwvhgqxqq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkivdfug.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gnhtzlgdd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyfszzcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gggsprrcp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqbkpmx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwfjwzjo.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrhidvcy.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gozenittx.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhoijdth.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guznxmlch.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsvdioml.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfvjwewc.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gqeckhedo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/goqmudwwv.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhwhjlqd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpzpvgwyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrtsaoet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnqdwzbnj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajyogvbm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxixhcwb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpclaucd.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzhtggmx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiacncki.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjxsgkvm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gvetmkjog.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvfiqrmt.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkazjjy.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gnttsdzyk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmkhiolbb.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gbsclswgv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhuyrngk.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsmtfvkg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gocwxskmm.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gufurlemb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobhojrhs.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlhcmsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gndgkqdwa.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjfnzbasx.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwdjmhlu.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmkwseed.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjeaxnqh.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gzyqzhllx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gwtjsjxjp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgwogpkb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/goaodupeu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsyrhzga.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/glqdwkdop.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdocbyzpb.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/goedkvmyt.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbxbghsq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnbyhqji.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gitnucsoe.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gejcgsyik.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlyncwgp.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gzvsdreji.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gsqalbdtq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfdzfxhbs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gbldkhxjk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gzkdrprxr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/geqokalcu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmobfrobu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gawapsbqe.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpsbprwa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqxfrqno.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnovsibwp.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/guyurrpzq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvabmihjb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeqpgwep.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwnshxqk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtnvzbdz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gyuhpizfq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grptlmckp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpuolxkn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskgklzpt.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvetxxfpg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmovuatp.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/goffvxtdt.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrbwirvz.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzppmrai.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gidsmtdyq.sHtML


<!-- 参考信息 -->