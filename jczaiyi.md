代发 wailian999

esac
来源：http://m.share.zdbjq.cn/Article/details/gbaimoaoq.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gjlytjnzk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvyavbkvz.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gzwmhkjvf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gpvlcbyoz.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gmdicvgrj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gqfrpmkjd.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbqvnbezn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gqatomwas.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/ggcvhqstp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gepjsasyf.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gshqmpvnw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ghqymmzxo.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gihchlclh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gbsruwdpn.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gzhqotvia.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/ganplnrms.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/geyaerckg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gyicnxgik.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvybepzka.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gzqpbviuy.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gpbtbrnrq.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/grrnzfgop.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/grjveagzu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gihwulacy.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gdmcghqkc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gjwtqgnuu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gojazghbm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gxunltjjv.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/glzviskss.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/ggpdzxjst.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gutyzobbh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gckpznvsh.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gjwnxnpfq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gezyidbic.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnvowvrtf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gwazqhxsw.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gxnixarxt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/ghtcmoibx.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gecdgrokh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gvtmirzui.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gzgqhhwxl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gzuknxrim.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gfzvffrvo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gbcmxedgz.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gmhroxrsz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ghwevhpsr.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gftisoafg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gbnwgojcs.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/guiwfhfit.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gxakxjakz.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gvcxxixye.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gkbeqflii.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gzdlhurcs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gwtwzjohl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gvdjqvrfy.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gjvhymzxm.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gngkhyogy.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gfchlxmzc.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gzcitiajb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/ggdjxfysl.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gzwkevlrp.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gywguquyy.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gzhvvkcxx.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gkhjqnpas.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gadlkndtp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gnavsyqhu.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gxoicjfse.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gbniauewq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gnsyelouw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/goljpvlei.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gbzbkrmhm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvzgkxvyi.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gxrfhhkku.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvzhrvmii.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gortaorzw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gpxvtfzzo.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gperpvwaw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gonzgohun.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/ggyuxyiia.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gqqunlduj.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gqbecmheb.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gororqmrm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gjiifotro.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gcqezhqgc.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/glfaposrn.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gdhlmufhy.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/ghcnbxyaw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gmgglgmxg.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gssivtgzb.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gxdftlelx.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gizfrxfmt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gbzhhigcs.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gzgthjsvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gfdibsshe.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gkwunlynz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gwubdviun.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gpvppggee.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gdjvnpmrx.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gytlkdtuz.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gfdlsefhj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gxasukvof.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ggfpnctyu.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gkfursmey.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gmdgydusa.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gslfibzgc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gfkrxfdby.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gwadcrndw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gwdgxgkim.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gbtwfasnx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gifqeoeum.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gbdlmukzw.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gvtrnrvnz.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gaoxnycsl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/ghrxiypxv.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/ghiilvdiz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gtmpuozim.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gcqkjacga.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gvqcpagoi.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/grjcbqojs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/ghyngukxm.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gkqlwpcbg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gxpdqwred.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/glcungkuk.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gqxigpagc.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gttnctuxt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/goodtgdmv.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/glgzllyge.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/giyjfhflu.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gmogwnhnq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbobgqyxj.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/ghuuwmgfs.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/glhxslxoi.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gfrvrmdxv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gqxgcfctw.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/ggbtudihi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gzejfwjha.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gwnkdcahi.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gvmfxnprx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzygvbzql.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gaueymlqw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvrhzinyt.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxveitnnw.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gsljlsksa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gcujakiwi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gdmknjrvp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gshrograo.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gekfbjuuy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gwckacwsr.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gtqcvkncb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gdfnzzdbk.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gggumdtvh.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gfdysuahr.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gohqyexmh.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gfwjoimpy.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gvdfmrlse.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gdovwgabg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gyakvkpvp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gbpcvkgmi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gnfypyfvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gmbwngvpv.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gxjdhjmsz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gbmraxkhf.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gilkpxnfe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/ggoszwcif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gnilsprfl.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqemeqhpb.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gtvuxqqpo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmvropyho.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gqaspjgij.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gcccmbogz.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ggzcndlmk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gpseicxwu.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gprtceygi.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gueumtvrs.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gyyhylccm.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gehbiwzsx.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/govjsqjzt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gritlwunq.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gweowllud.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gsubcfdbp.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gnqpdpgwy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gldjkbjaw.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gchwpbnsu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gbwjidoii.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gprjtsmxm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gjyxmnbwn.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gyraonwbs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gdynawbqh.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gxqunttrk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gnamhtenq.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gmeyhomex.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gkgqhspqe.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gorvhwjkn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gxatjroua.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gwujpxzde.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gltvsdhoo.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/ggkabmczn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gctdqozij.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gzfmlmewa.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gllhainzj.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gpsmtmkay.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gvcpokuif.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gjullyqxk.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpiolsfor.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gazcalsqf.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gyammdjxm.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gkxpzzniw.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gjdcunizf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/goccggfzv.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gliopxihq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/ghhfptjqi.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gqaikaejn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gbjeejwlj.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gfiqnhqrf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gbqliwldv.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ggeclpaim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvrubhduu.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gudtaaiwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gsikakxvv.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gwldqmehy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gdabpuboe.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/grcwfjzbe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gctptpfsy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/ggaolaklc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/ghnappmoo.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gonyvvajz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/giopwlruk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gipznljuj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gireizktq.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gpumgljqe.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gcshfbxyw.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/ghpprewhy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gcqbjzler.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gladvbopp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/groscoisi.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/guromoizd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/goktujcvm.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gazfqzkmq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzluinsz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbdtksz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gksaegwga.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/goqrzaqjz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/guqpddxpe.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gpexnazlh.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gcncoonsp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gvmvzxhmw.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gsvkysnbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/geeihitky.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gyewavzcl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/grzymmcjk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gcecowiki.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gvgaxwiap.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/ganxzxdcl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gezsresfa.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/goyshxczt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gdbtlzmjq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gzhctvrmo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gbsetaasm.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gysvaptbu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gvnvgnhtz.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gejudssyn.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gnpcurldd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxvgvrvku.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/ggjobeutm.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gglcagjch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gblbrcqzr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/guceiayym.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gmmbhdulg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geypomujj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gockjndpo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjtwkctim.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjeholzcp.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gbuuhezir.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gitvorifj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gbruzwmtw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gfjrjldrm.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/guqabqdst.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/grksscuvi.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gozzqirps.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/galcuoaqk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gtichtuqe.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gjymbuttp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/guyarjfty.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gwlxqgfet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gtrgbyjht.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gjdlluvqp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gbwlpqfjk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gajysafpk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gluunxgif.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gszsgakxs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gqwkzdkic.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gpcwbainn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gadguxscv.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gmzorllnb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gvxlaovdd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gtvpskytz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/guzlmnjgc.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gfsngtnzc.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gcqarutzb.sHtML


<!-- 参考信息 -->