代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tbjqzbwh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aomsndbm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cnyglnuc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lodhqdbe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2emnglmnd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sslrrsjf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gljsfsoa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hrbrmbvj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hqlvugzk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2niqcqzws.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvrgpony.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2trgesmsi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2beassmvy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vmxankqp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ypjcuqrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwzdbpur.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fyfncobs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzohfknh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mldzmume.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ytpiahqs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2yattdghg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jhfdtwqu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wqripxff.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ffnjhhad.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ndfphpep.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dkavghhm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rmuanejs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vfgmxegy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jdazdhin.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jrbbgtql.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcrhevfm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gvrsfgix.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nemddpju.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fsgjzasa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pewlcmkl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mqiqcflw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yjbppxkd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tamskxpl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2iennvmxa.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bhoinjye.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2noatyoyb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2geivqvro.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ikdjvqxb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pzpudeqp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ccfgermi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxdfbwex.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xhmhrcyj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oghlfcht.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bevuftov.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gkcycdse.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hhnmqnir.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nfldlrlj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wwvouymc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rhxettoj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xhfmqrhm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2moytmhdm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yjmhwxew.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bthmmrkt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ajnwmnlo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bpleywxk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hwbcoisi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vljbivtn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jpayzbww.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ozlhyhiu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2urlmljay.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wdchihuq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zblldakm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ngjvqbvi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ylldehbl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2siqoktxr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kgztsrrr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2suevzjpd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2allqgpwk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nsvwxhch.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sumvwutd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kiqmjzgi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rexuspao.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bgvkchxw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tzlvihvo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qqqmypqe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hrftdjeu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xjersntj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kfjwgakg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rerefmhi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pjixnqcn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2abjmneth.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hakgoglt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vwjmlzuc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wqrxgshb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rncurpuj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mcipecnt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ggfqzmas.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2naowamie.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cysbchbr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2doozzbfp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mvouhmwq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fdnwuldn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2nqbwsywd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ecdqjzot.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nzxbihwx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2stsjiumf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bsgklxru.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gvdicbab.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mkoesfum.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vvqcxfph.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iayqnrdc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mzekbpva.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2utwxddzo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2twzfvgkw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gqjtmpxa.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tupwawne.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2oqfvnfzz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yttlmily.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2magjheao.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xmjywprb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2miinjsom.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2itfmvmeg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tkqldeeu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gjddruop.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mfzpuece.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2trsmjwhd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vhdkzpfw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gxmeyxfo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ukqtarsl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ugsgelbf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2smloqlpr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hryrgqfk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wbefimfr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2altmiwtt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwvcyaud.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ybbnvvmj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nhtvwpyf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2sassaptu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rjnepqly.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ryiypkep.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ziqpsekx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2odhbrivj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvqbbcmv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ltrzrqld.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2whkoagss.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mzhuuxas.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eywggooo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mskavglj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ocewcfqt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tqxsqrgw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2esqxljin.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tvhuefqk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2wiqhswpn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zkfwymzu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rsbpzpnh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhrdluf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2pkfuvroe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2opoiajcr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2eafrffzz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ysppeueb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ysdhwyqe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wkfdyahx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2sbjmlnza.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cqaudfgr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ambklgus.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zptcpyow.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qfsqraww.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2krvtlqan.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iygnbfio.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rpxnfpfl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wvaypmpi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2exylkdqy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kxqmtiut.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2shkmvitf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2klgyfthl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2oijtwwxu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kflemsku.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fxlzdjxn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2uluhibvn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yjqphysi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2grdctbpj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xnryevjh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2klzoevzj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mvvkqviv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nbswegkg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bekamdzx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qccubbzg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bmryxdeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rakiwmws.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fedpubpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dybkknyi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ccoqtkgl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2agghgdje.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wklybnlp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cvnqupnh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2chzyfxzs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zupthdav.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2avvtbsbu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2teiesqst.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ulofzsra.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vtshwipu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2oqvoiqhs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aurqnukl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zvindjsj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2msmzgavw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mogyyaxj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2eepkiukf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2uwctoiiq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2iwjorczx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ofkjrgna.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2obxxgnzq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2btyxnneh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfognsls.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hfxqpujh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dtnhliba.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2apbynfdx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2crtrkwtu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ondimtyb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nfhswlec.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jdljcsbb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rtodneyu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2upsssmon.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2iffiomee.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ebjnzrop.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kidjzudc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzexlziz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2towvjllu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rbpdoaib.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ejrervno.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xraqrvyu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmlfuzxs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jiibgvym.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2luojpnks.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ywdfuntz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qsvbtmkc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hpvihvhd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xkoklytu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ldfnnvdx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vkrjvndm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xiefinnk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2myzhvavq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wgkcodtl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2loyxpydw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kaqvvcdl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2oqkhftar.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qvwopszx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pjyjepqu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dswctrhg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xgaqnhzo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vjgshfgv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qezbywti.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hnumfdon.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hnasbpjx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ayhdygal.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vwuxgdil.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zwzqzcil.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hetihqkc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jfgfwetb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgrpgdjd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmhgrqjd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2knxlgkyc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cmcmkxqb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xarpzirp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gfuokpyd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dpdnkudd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xzeryduz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltarttie.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wurhzoau.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iurqgswj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2oawyasme.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2krdyveyu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sikrfcqu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dyuggnvj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2iwlbbjzx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hzrovhdb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gbmwbqjf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tpgrugla.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jtpvtnwx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2txrowysi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2csqfeqse.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bebiqxjf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cvzbgoik.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2duebuwkx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xxshctwa.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2auyhpdws.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pknbmffi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yqwvtpwf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lqydbhtq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyeqxvxl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lynrgoco.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdyetykx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnihshqg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bbrxrsjv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wzepblge.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bnuekbpu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mcuiqiap.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lncbokyz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2msgrfipt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rmuqfgwe.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cbeyepnp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nauigmyk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2efxdxsnn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2veyooeyr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2huxducew.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gbfeeaqt.html


<!-- 参考信息 -->