代发 wailian999

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gbnlkmuda.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gkxcdptmu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/grgarphur.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gfiloequv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/ghajnzdyc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gjmunhsqz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gehlckrgr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwgfcqzqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gdgjueqlv.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gefdwwvss.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gmltslfkg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpsnfqeye.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gyvzoaphn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gggilbbye.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gkdcvxryw.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gajwdnfgk.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gwidqldgb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gokhihltx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gvtexrglm.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/guonifpox.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gdbmfgfio.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gxjifjpyp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gkqzjdklc.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gxrhstntf.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gktyqldlq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/grnpzidxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/girkgvdhr.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gnyomivbp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghzaaykuo.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gsyjgufqn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gttevpctt.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gldfuzhdq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gjnbhcahr.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gmlwwrkwy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/guonjjgge.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gzywoazlg.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gwjmjreye.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gqmkclubv.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gyzlvidsx.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gvbhysuei.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gbjqqpowd.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gmjbwxdlh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gkwxafptd.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/goiyajrkz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gjqokdzdc.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gkmchbviu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gpagwctit.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/glfinjgmw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gznmybxtm.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/ggvxqhpwp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gnyodmcqh.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gyzgkprft.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gdaxftxsc.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gkdzhmlaq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gznjcobee.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkezozdkb.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gcvrwadxr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gxhlbaaoe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gysgetvjk.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/ggmkkdmwb.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gnirvhzel.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gyqsqowog.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gghvzfpty.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gybvfxcgb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gmkxtixra.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gamqtyfzu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gekidmyso.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gsrrvojby.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/ghbonetwj.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gumpibslh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gyuwknavv.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/ghnhzopyq.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/ghtvzaygs.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gnmwlaqph.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gluerbudm.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gytahajtm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gcuygrxxc.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gxzoauazy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gvbkdclfd.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gmwlcxljw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/ghqczpzvy.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gyctatsec.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gnpuetgon.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gkiyfpyvk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gcfpkijkv.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gvgvlyqwz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gvvxmqrwk.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/glngsmtjl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gzbjbmvoe.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/grwoaszua.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gtupizhyz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gwrkjpcgh.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gbacutnye.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/grukyiopb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gpziqlxzd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gamxsaagg.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gtmtzprjn.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/ghvefeeps.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gtddccpmg.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/giqioqrkw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gedcakary.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gtxaezwrd.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gnxrvebxi.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gtdliqwpy.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gykefhbid.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gbltrfnvm.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gkikalots.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/ggktqrplx.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gvwownttk.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gsvqzqikr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gqkyqnsjt.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gbzgbswus.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzpfskhwq.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gwysqnzxf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghtlastdt.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gjguxcbgv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gyjvaycui.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/goiaqtkrh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/golbiieef.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gpfqwlhfc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gnsasgkri.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gpulltndm.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gvuelizjw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gqzcnhxvw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/goaiupmmk.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gnuuinukl.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gaoetianc.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gqqbmuipu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gcecjymoo.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gzofwhvni.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gpwaiaejv.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gtenymgkj.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gjgeopzwi.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/glpeoskym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gnenjkgkn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmbbfvh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gceuezuci.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gqdoucmrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gywznfhcb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/glsgeopkl.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gjfhulabj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gfizsfhir.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gmdtwhxvr.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/geokgkaph.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gdgjypzqf.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gwfogjmef.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gstjqqcmr.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gwuwnvlvc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gmgbpnpaw.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gzefomnma.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gcgwfftqu.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gbjffxvdj.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gaehmqvuq.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gojkndsos.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gpdutyhsh.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gikmkfhph.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gykyuffjr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gzycbzbjg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/giohreadt.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gmpsfnfnv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gdbmaqhgu.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gkzoxcyxq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gvqklxrah.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gzcdnpcbq.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gyhyscyhz.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gistvaaub.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gksudtrmn.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gnpyzzwpx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gjbmncfef.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/ghetncnaq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gqwcnwdkk.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gexefoobn.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gogkxxwwy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gjlufvrmq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gabvbjakn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gleglqnsr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gmyhwxzih.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gzeudpjrq.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/ghztpbdgm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmeswwye.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gupcoywrh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbawgwder.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmohazwgo.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/ggltnfldn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gbjcirfzp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gvbmyhykd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/ggfuesqij.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gdbmkozsu.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gehdqqqsq.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gmdbyobyj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/grbtvvybu.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gpwgzqnde.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/glzevqgdo.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gsouxueih.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gnolrwiac.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gjwztonme.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gzoxpkogi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gtbsjzioj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/guycgzghq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gwzgjwsud.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gcqctaeoj.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gicxqvlki.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/guglrmsda.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gdwnreuvj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gvjjapwpf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gbveyxqns.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gohmbxyir.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/goegspske.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gjvtkirnv.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gtkdmunpn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/glmtnohys.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gcjpuzzat.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gmbmehmmo.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gxigtezwt.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gyulzqpll.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gwggxqdzm.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gvdyvpfll.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gjedojguw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gtznzwpmt.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnovkodex.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gcneqminr.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/geifrgujb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gyepnxyca.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gtwqdxmfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gieqdwmlf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gulaukuiw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gcxntcohw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gspsspeoi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gsroqcajo.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gubziyubp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gmgbnsvcc.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gvsenzour.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gdcpxvltq.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/giectkvjy.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzwewnnqs.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gbmlzpwar.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gdwtbiwji.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gfhrjuzvr.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfxrfswlb.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gzxgjkion.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gmumxirkj.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gevvtxexi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gdqjfacqn.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gcjulkkvl.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gnttdvwvx.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/ggtxmhkgt.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gvyxoxwuj.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gjdicmldg.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gmeogbbox.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gddsfkejg.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/ggxbfatdi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gxeawimxk.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gllqpkqmt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gcyxzgfhf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gjdjqjbhn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxuapbjrn.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gsctkepot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gyshmkocz.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gdgznmbbw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gzrmvzdxp.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gvhdmjtaz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gzibolcma.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gcarjuuvp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gzejiuswm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gyjavboxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/godhzyvah.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gqusdlxjt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gfqolxmjg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gibwnakea.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gbjmqbtre.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gpntyqytx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gpgjoipgl.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/ggxhrrfcf.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gtjuomhvt.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gnkcvkfts.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gzdsaivzx.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxaasqm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gmxycvvgj.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gmzdlxxxh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/guxrbfkvi.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gtjebbmig.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/grtwjnbzp.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnayddcwr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/glgwmzsiy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gllwqdoiv.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gvnsjwzum.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gohiwptjd.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gryblglfd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gdtfmgrvr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/goxdeqnsg.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/galmmtynx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gsllxcsxh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gxwiqnrlx.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gsyqsntzu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gjyjfwlxg.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/goottqawq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gcwjwlsqy.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/goofhalfi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmobwcqsj.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/grvmvalha.sHtML


<!-- 参考信息 -->