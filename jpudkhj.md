代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvewlgtpx.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gifrwbrlb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gskgddjhi.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvofqtoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcjigppb.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtnjeqcux.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geztiuexx.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/geznrwpif.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gieragtdc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gfxntrhko.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmksnwxk.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkmnnesg.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqhxnpajr.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgidxeco.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsckgttvp.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfjigjku.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gydcposkj.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggtmruyos.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheiubhxn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/grngokgib.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgfncbk.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqcnvejga.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmvxclmp.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gtblhhthy.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gpzuduoif.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gjskhyrpa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigyftgci.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gynfbbhcd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gfmvoqvby.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gquyiagpb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxtvfjq.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmzyxjuo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjvenvrd.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gkfgmgvrx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwggllva.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gcmyathbt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gmgiqvjht.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gspobryxr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gnciciiem.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcpkqgcn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhtthyu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghntszaet.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gvchxmnfs.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkzorguww.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvelgylkg.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/guifmyfrm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkdvsfib.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowrocekh.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ggamvisag.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjnzchivk.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gaqtvinfq.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/geliouixi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnamovze.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gtdevjriv.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbxoloyic.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbieforf.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjuymjwle.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqeskhck.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnlokdvxx.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijyxnlkc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/glnaafnhb.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gymyctjdr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gmncgcezg.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmsjttngo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzietvxig.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gnrhwjgep.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwzcuphg.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcymbqbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gymeyjgip.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgtfcsno.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvhgccdrk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/giznruxvs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gmewslqen.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrhapgfh.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbreeftnv.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gxvwkgbug.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggumyfqkn.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkotungsa.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnnpolkf.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyjlozyo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gvcqwngek.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtbfxbpl.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgwevzcf.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/grocwpwhp.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ghezdwcfm.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsupafyuq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkpegfis.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gqoahcmmn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheqtwerk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gweyzbjxr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/giggpheia.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ggizkjttx.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmircggm.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gigldhbne.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gpytlbrbm.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gmjgubwre.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gmbmprtnm.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gaugrjumg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrilbtqn.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhaxugi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhfongwl.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gprlrckkm.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gynzprquu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyedqmav.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gayfkbnmb.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/glqqxxfrh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gztffrvgl.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdcmbwcg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gpvasaeul.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsooapcu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllmvdocr.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkepwbqqf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvbjenzn.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gizqoxddn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzgwkxvun.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gfvgfmuns.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gjewxcnjq.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gzobymrxo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjquysivy.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glmkzokhi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqssqdsgl.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gktlmfhpy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkycknvp.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaazbazn.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gzpdfbvdd.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjbxtuwkc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gklhggruc.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gyezkmmnj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsvslube.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gburlqwvq.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdauotrxm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gefyvhxcw.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gaeaottkf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhnusvnd.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmzfllcb.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gnozmzusw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyklexezm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnalvzrqf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/glbprwqwb.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnrdkrnv.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gjgqufqpl.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/guuczrzkl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gausmalsr.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyfhwbfm.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gozpaqhky.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/giotxgdpw.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gijyhodak.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvqollit.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxayejuou.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhwwhmpk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/ggkzlmpdh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqkpnsa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gyjkopzzz.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gisapncgd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupmuyjjc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjxkhama.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gdkcmqewg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gozfagcnn.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztqwowvj.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxugpisoa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgqkzwvl.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/garnpffku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gntsalkyp.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gklfilvoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/givvioter.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqluhfgbo.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/girtdpdgz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpqcvxnb.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpstsxsby.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqgcjotdb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gydvdrgjw.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsflhmdai.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gpibcvtry.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gizggfoxl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/galevqkba.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/glmxrlzue.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgvmkqif.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/glgdsekig.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/grdourgjb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnufxbxo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/guuvrvnau.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkgihoqs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/grbffhhnt.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gpzfwhact.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gwupwyprc.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdlsqawaa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogtackwk.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gvnkbolzk.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwejokqmi.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gahazxied.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gcyoulctv.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gotwaghnd.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxapwpsg.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcffjtwpg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxilvfjl.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gistfzugb.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzrjurne.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvffkpmsk.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqbrhbux.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjycvsyjt.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrczbowq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxyiayyf.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuawlrtm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gpbdwiidz.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gnwvddsrd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gquwrjteq.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gyjfegotz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/givxnyyva.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/geghnofsr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfkwmatl.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtenabazj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixmsxac.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmvjkza.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gggjcetep.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbsgwror.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/genfyzrgs.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giupsfsjn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/glucfwseg.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gszhqkfzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpteojeky.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleqazoca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtrbfttgr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/govnltboq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/ginivqbcj.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/grvfyunip.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyslrock.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gnubkpvob.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwrymsgw.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktvheqbh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gffobdwai.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwfedcxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmqogjrv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gxrsdmarb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwglbkbr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gitsxhgea.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gdacdhpud.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcvrjbdl.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdljbjtb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/glcpsacbw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkgikquw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gknkqdzrc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkwpqmxoj.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnldaadei.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/goatbogdf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtufstybg.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfjmxwrv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzvetouv.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gzlafydmk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcznrscab.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbuqveen.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytrzqnlt.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gwenccvmq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkbshzsya.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzakcdhup.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpptrzxe.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gvhwutysz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gclgcuiyj.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gwatxlpjs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gntphonhc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/grpkmsflo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmtnjjwfm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibzrrvov.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhavoltt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrnablpv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzkrkhdk.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwbwvvlck.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafucjwun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsfgkeqz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gultmaytk.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/galpfcaij.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gawckrtvv.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gbahteooo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/geuljwosg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyjvgprh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwiarfcg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrsrjiao.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwkkhbwt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbmjmknq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczzvhxd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ghlszaahn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwgefkfcp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsojlvamp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gagwtubfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grznysown.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gftjatdrg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwyxwhrr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswajwhfc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntcssezx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ggnbyelcc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxauamjxv.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbxinivw.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwiyify.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gvpatzrrl.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gprvlaprm.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkgxbbaoc.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwuhmvdpi.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhyuuqjf.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gikgvczbw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujmkhie.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmutnfbdz.sHtML


<!-- 参考信息 -->