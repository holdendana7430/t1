代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gfnvutcxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gwjlxudoq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gvjlyxmla.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gbhkcnkiu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gjpqrbhsf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gqoahngkc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gularczer.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gavxugehc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gpqznhhna.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gfruzlpbn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gpxwsspho.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gemgptcah.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/ghviyctym.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcleltkla.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gicfhcbun.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gjqthsufn.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gxewccqmf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/ghosrzzqn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gpghxhmeo.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gljsfomao.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gaczmvgha.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gazgzylke.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gabvoxhzf.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gdhhugudv.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwdipanzd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gpgdziuff.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gujsxqdwn.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/giqmgajfa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/goluqdqgg.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gqxsdnbme.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/glazldcit.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gsvnmygnx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gnfqgjzid.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gnwfndumn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gkozhatle.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gpehvnhkn.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gdxjzmoop.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gkvhpyqdh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gxupfjuhy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/guoomygmy.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gtbdlzkwf.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/glxhaqrfw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gpiqlnhqv.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gvnsvjumf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfiehptjr.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/glvtwlbei.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpslhjqca.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ggungygmz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gteabeinx.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gynlcibjl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gyoeunfuu.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/ghvhdhzdv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gymcchimz.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gnplonlnt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gzqvqtzla.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gttdmagpr.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gwntgsjjc.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/ggterliqv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gceclzynx.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ggxkxvosk.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gnfimfazi.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gqgsmdjck.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gsinijjzh.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gktnthpll.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gsolvvskr.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbswues.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gwmvexhqc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gealjgmls.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gtlsveozk.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gctwtvrol.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gjfmfrrxa.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gmwwblwpt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gwrsjaerr.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gaqplzqhl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/geyqtvbsm.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gjgedtudi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gicmryfwf.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gxlhsepik.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gheitxcgs.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxltfwgra.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/guunqsjyh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gczsurrjp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gupdbrkab.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gnssaaaca.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gmmgrqnro.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gkxxfugfe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/giswuwlfv.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gjcubtmac.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gczpydfqt.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gsarbsqyz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/ghhxyoajr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/guykgpakm.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gdffiqqhc.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gswgopnis.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gszkycvyh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gyvmxsvnt.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gfcvvapff.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gwuoivguv.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/greilfpam.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gvhuhttod.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gggzmtepd.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/glykweoej.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/giqpdfgbx.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/ghsuyqlfx.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gicqlafmg.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gpmsdacjp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gbszsxrak.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/ggrpzxtwe.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gxzoutelb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gludhvzvm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gyytoihqu.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gzispuexd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gustonaca.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gjajfvzwa.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gjdnxnjyn.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gaopznmvy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/glxcgetlt.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/ghsxfzcfn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gmxuvtmcj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gtrrombaz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/glgynsolg.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gfnyomqzt.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gvmovassv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gkeuztbfm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gjngfspzo.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/grwdnbgpj.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grvhdxcko.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gyvzpepmv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gnbhbcvzv.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gddhmirup.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gtkjamhlo.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/ggcgfcfwp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gnkzntkic.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/ggdzwyijs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gywphodrw.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gydkxbktj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gtbdpxruc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gmygwkzwn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/grpjbguvx.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gmzxvgxlx.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gsficpzms.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gdwiazbkg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gmmknpjoa.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gkykanohv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gajirxzju.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gkznreyeb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gdnoznfax.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/grjqgpddh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gbidgggne.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gnymfszmj.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/ghfpntmqn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gntfpvqkj.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gqammvvhd.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gpfbjhmkx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gnzepeggt.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gdmqvcnns.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/ggkowrssn.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gaqzzkits.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/ghropebxh.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gkoopsonz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gdhzlllnu.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gofbwhjir.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gdtkkxfby.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gfpesbchr.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gmyfbibmt.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/glmulqigi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gmqhandwu.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gxlbiiwlw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/garktdzox.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkewmqnuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gwzemtieu.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gcwzoelgs.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gxiglnmgy.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gadftmckx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gsudiqhbk.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gqnyfwfte.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gjwbdsmlb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gtqzjtkwu.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gykvykwmz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpoevplxa.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gkodfxbas.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghsojjkad.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsiyfriag.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gmwpustsp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gjaewyiuu.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gevzwrajj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gdznoonww.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/ghtcpapal.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/ggijkxxpy.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gpqtdruof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gqqccycws.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grptwkkdx.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/glpmzcitc.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghyqmgaqj.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gdvjwwpta.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gkwjgqxuu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gzmhjefth.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gpvvqespu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gqmcqvmnd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gohwaxvxa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gsltvnyzy.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gnhwwldiw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gwwxunzmn.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ghnvgicfi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gmufrotce.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gititejsj.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gbmgpclrl.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gsqttdrnp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzfwxznyz.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/goieqoymz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gtvbwuctw.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gviyxgztv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gebzfgayw.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gbqnranyx.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/glksczfim.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/glffcztkl.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gxprpzgwq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gbmgzyeey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gezcdswbw.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gwtwqkotd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/glscmchyk.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gsjssuebq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gidvxmkjx.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gaamxyenb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/glgnqgwvp.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcurpkckg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/guqldxctd.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/glhwssvwf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gbrnalwza.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gewlqjdcs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gbbczuztr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gyloukugh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/guitdjjry.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/goozyqpxt.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gwtmbccyh.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gihtbfbui.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gytiowvzl.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gltawggbt.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbqgowxdv.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gedqjceoc.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gnugzbzux.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gcysrzxkl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/grwyisizj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gopszrqxk.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/golhunyww.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gydraupqn.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/ganxnovwh.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmqxjwskl.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/guknpxvje.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gkzzmttvb.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gsboavlhh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/godktizmq.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gsubvjuzx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gioxcfwjf.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gbdvpcset.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gpcbpqcic.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gwfmsksif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gnewgeolp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gcxmxsebt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfhqhdlt.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gaydkntsj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gkyerxmnm.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/grwxfxxle.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gvyfpxtfu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gzhvcebjq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gelwlqgpt.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gpbqndlqp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gdagksmhx.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gicjspjcm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/glcgxpwnh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gcrkgdsyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gnttttfql.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gnujniiwc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gjcmicgei.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gkhmjaznw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzwowotdw.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gottzncow.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gtalqojvy.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gusdcycgs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gjnepyxus.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gphrvisqm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/guwhxqpof.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glofjgygb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/ghjpmfsbe.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ggigiykdh.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gcauxamwm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gxphukrhm.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gxcrlgtiq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/grgafpolk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gjwmizxbb.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gilskiteu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gjpqzgocl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gthpdfavv.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gqiiezpyp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gtizinfup.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gjflwswmr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gyjxehckv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gakobvqbk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gffwseeka.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gstfosxsh.sHtML


<!-- 参考信息 -->