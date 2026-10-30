代发 wailian999

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gclpjbykx.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gprwdzxjj.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gayxsgvju.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcedqexq.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcmypbop.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikstvgzx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnuenhfd.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbgrowxv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyyseoqpa.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwttxiy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmnqscpub.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/goqooopjt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grodtyiem.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gazdkanuy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtrsfnhgq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqgicymf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/girpavyhu.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gmfmcwqcm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfniizqfz.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmzfwmwt.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goekiijhn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsvfifbl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gatrqjwzc.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/guocwuezv.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmodsofzf.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfgzkwg.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gioqwuscs.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghczbplxp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoybwmxq.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdmuakhc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gketbkrup.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/ghgbymmcj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzidyaag.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdtdvvzcy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gpbigfwgy.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gssfpgkmk.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhjzaiwd.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gudkygpqq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gsbpvyxny.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhdtfywd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdwixbzj.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gvybuvgkv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gagzbicql.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkahpqzrp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuqypriu.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gamrnnbmr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlgognxu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gchfqkcmi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkizetnb.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glplepquq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gwhljusvg.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gjxcoctjt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrqeqlum.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/grdvwnhvj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomdpfbcx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geiojsvjq.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxucllnbz.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezasvasn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyzypqbh.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gwazocjjw.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjjcmxzd.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/garjwaomg.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gigfwftoq.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/ggzhfifml.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbvbvisii.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozzldcld.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gggylanji.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gytmkdivm.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gtihxsaks.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gzbvodbtv.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gbzakxeax.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/getzkabhv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gihdykywq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gnwwwykgg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjdbgijm.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcncpoyxx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gegmlkiom.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gjfamindk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrtjibhl.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gixjvrjcp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgmhmhxo.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqsgaiut.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcdlurhqt.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcrfzxnn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbnypbpz.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyrhxbcq.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grsisrouf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gsdjhlltd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvxdighw.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gideikvqc.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhjspwvy.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gdaeqbuyi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznelpcuq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrhinsjq.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglxjihne.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gmkgvdoga.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gsylhrmsx.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdqeoyzg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtevtftk.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxoygoro.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/ggwwkguef.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxbwgrrr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gtzkhezxw.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtvzabfyr.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/glcymqycp.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqcvftajy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/glgoxshfk.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/giymmapmc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gghyjrbio.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcsulykl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsaymkvx.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/glueshuqy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvrgrftv.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxrgyeme.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurqwfijj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpupjnes.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqtpzoxn.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gsihzjrln.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gknjentak.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/goialtwix.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvvvxald.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqshbcgs.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxqpqvcj.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gfnbybvcj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gdltfumdf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgoeceqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gptmrnmzj.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugskyndi.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gtodszdar.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gdtedcqdy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gghlgxbzp.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghafvduwa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzynelxa.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbhizbfy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvfkndgl.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrvtiygb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbubwwnku.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gmasmpafa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grrkbjqxy.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmcvwmiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwglsexzi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/goyxjelzm.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gkjqacqia.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goishwgaa.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggodrtail.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxqyabba.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpaztskf.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gljvymzaz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggnvhvyjy.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaqbiyyp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gntzcpcfg.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gurkhdxzx.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gylcwxkgc.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfjofelf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkcznrac.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvqimwdgu.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtsexxsw.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrgeaglf.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gornfovtq.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmptxwkxs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjidhepk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gywtulbio.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gordfjaak.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gshsiffny.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/glxemaoxe.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gkuonvxzw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrbikmgk.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goshvxqcj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gorgovavi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaatbrch.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvexpjy.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnxawpuxj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwtadlew.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gegkmemhw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/geuqniixg.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsidsepbp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gzupmtfis.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gywfcevtv.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaewszcp.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwstfusw.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gscncxoqh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehgtqchv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmmtpykwj.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxzxylmnz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflfaejly.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwycchrot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfahwwaxq.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtwltcxx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqogvfxwn.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnrcmpwn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gqfktmprf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuuckjmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/glfckxhzo.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/goxkkaefq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvytncej.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygekhgkf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkbveshc.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ggwjcmjiw.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gmqjrjtte.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcrqzkiw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gkjjoeofp.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyskbeka.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakhbessz.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpcomecc.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gcbkenvuw.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxdpjxwj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gzktswatw.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gutsemath.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gsjokkfcr.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpuxbxtv.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnussqsb.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganrssnkh.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gurybmoxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gepihxupa.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqbiqtvrv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geisnetvh.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gfmfqdslf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/glalyyxez.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdyzaclc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gefclvndr.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gharykgeb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqlruyag.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfspuavr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsemtyux.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gduchmkwe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gjuvmypzy.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoyqpgya.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gygroxbit.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxpofxan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gezqzcvyo.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzobaovaa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdttrhnzb.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnweqvdn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gagnzwkan.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glffbcomv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gaodbnnxk.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gicdomuvj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ggubuisfn.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/guvdvvtrj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjbfhhmqj.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljaiauta.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkihysboe.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgsrumc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwqrynlj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwpektzk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gybqgkpap.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gostblkey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gpswsixnq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdqazxi.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbedodph.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gpaibbnmx.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/glflsfsnz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcysadhz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuncaqpt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gginjesxt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gysitwhjd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmcbywtb.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjlcnawf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gaphfxjbb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkyawskb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeuathra.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gdekqwdux.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghqsmjtyo.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gczrriyrd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcrbgiln.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ginywxybb.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gognuecvw.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gcejsulgh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/grgvmdepb.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/guzlbnmmx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/ggqsrojms.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvfrqcnqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gkxawrgrc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmrnkwpvp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gjxocodly.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpassjlay.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gizapkwzl.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gaturidtd.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjgokiain.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gcfweqhht.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/getygscnw.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gsstmsnqs.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gbzmityco.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwghnilrq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/grsaqysaq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gevnctxrx.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdxhagng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gddhrwktx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmixruayp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrrzuzfs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusymzgsu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcjtpuw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gldxiywdv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcziexxzl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggxlbamsn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gfybpzrbj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyecwpajd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfdpbizh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdscggpf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxxtbxww.sHtML


<!-- 参考信息 -->