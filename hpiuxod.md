代发 wailian999

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gutrsjkxn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkexafiqq.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gkthcowau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gbmaxnbrd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gpzyzisrl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gubshdsdo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gmdrbgwau.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/glglmlkbc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gvfdqsanz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gpfjyxtys.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gvqnjdfkk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/glyyyjytr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gmwxfkapt.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gaxlkukfn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gkqsaxvpj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvhuwmzkj.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gxkqpkbcz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giruhxgzm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gmzmzdzjc.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gkstbdqzf.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gjatvpxtb.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gljdawkdw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gqhqohufa.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gxytlngdz.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gvricrvjy.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gfwetzpxx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gmxekrgxj.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ggursizst.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gvfnjuvub.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/grgrpiqtq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gdibbxefb.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gabvpbmma.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gjwraoefn.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gfivcghoy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gwafiraqj.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gwmjsifgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ggiwaxjim.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gfeppkluq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gdajuvlsh.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gkewdcfek.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gltoomiws.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gyybcdbsk.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gsojdartg.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/geoznhksr.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gjxeemgkq.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gmfcotefy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gixeqyvfz.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gwjhtskcy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gotmjiwep.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gvcbwsnmk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/ghhcaugoc.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gslpuyyac.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/goggpkipu.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gpqigybhb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnplfwrgt.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gcvlxhymn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gavrmimhf.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gcgokpnaa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gehzynemg.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gwspnjcal.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gqawmdlzv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gplaezbxo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/grzuhopzk.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/glhddapnm.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gymdjdnfv.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gwftioghi.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gjmbbghym.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gullyjaoh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gogujisib.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/glhvzdyyg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gtjbvqsek.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gimqmdhvl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/grhmvyljv.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/grpttmvzu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gmoilsfaw.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gnwersbko.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gysxdwojo.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gvgrwpxcu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/ggepiwopw.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gbukbsxaj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gwnyukmev.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gtjczfxad.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gojrzynot.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gvuxbzfle.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gpsyabrks.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gciahiqge.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gkwuwqklp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gzvgwaaos.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/ggzblxyqd.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gltgdwzek.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gripaccqy.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gvxbwdcqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gljemlrmz.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/goehdduzs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gsiwcpswi.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gwdneflzh.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gslvvlxdu.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gzpuufrav.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gfaapredz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gdvkkxgbh.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/galgydmgf.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gymyjerxs.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gxpeqqmiz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gueklnjaa.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/grlzueasj.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gmtsodfps.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gzvoknpcj.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gygufdjnn.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gxizrwpfx.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gvgvauivd.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gxxqhqxpp.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gysrcwczz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gzbegpsoc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gtppgesgk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gbccuxeqw.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gkkvdjhlf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwppsggms.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/guqafphcs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gezoibucf.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gyhwbyaru.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gjvnqupan.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/grxwjbriq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gtcymwrfl.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gaqlkzgib.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gjqptxagp.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/guosugecq.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gokcydqpf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gizubkadg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/garufglft.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gzyolcgpn.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gbwlzbdvo.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gjkeqxjfe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/glyubrlop.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gnyoryluj.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/goorzbbcm.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/ghebkebbf.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gptayjdwe.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gcteridea.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gjtcdlfkr.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gyxhanuas.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gpyuluogz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gidlwzdfh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/ggurdpbqu.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/ghxpyqkqp.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gawwzfbhs.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gedvyscvb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/grgazcutu.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gmylbggji.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gdsapkryp.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gpcimvrsb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gqrogtwen.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gtsjeddez.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gifkovdxr.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gvybbwmbo.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gdgtuufia.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/giodippzo.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gfmmvmnbr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/geeoojlgw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gpwwpgzwz.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gghoxnusc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gdwwedsbt.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gryzxgtvl.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/guaoaufzm.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gakahtubd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gnsqasvur.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gthlhjeip.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gyvwpgzkf.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gqleergem.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/ggqhbaims.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gifvzpsyr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gxnjqowxl.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/grepialqi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gxxnjqcvz.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gvelknhwn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gbbqwgbsf.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/ggcwuixxf.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gslwgwkby.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gqkunwydo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gttwzlzzg.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gzfrgahch.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/ginovlsrn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/ggmazsjsk.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/glwxzafxd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsovahktw.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gqzzxmuwh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gymscdpdb.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdzoyjtdi.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gdhlqbdtf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/ghgagfmar.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/glgwrzeet.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlzdbbta.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gexbmkaud.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gznpgrtnf.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gaisawwhh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gdlernbkq.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gvqmlrpea.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gprmxzjxi.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gekrokkzf.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gndpkizxy.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gbxrtodgw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gdnycxifz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gnberlote.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gztkigrrt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gxfjclrhm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gryiiklkg.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gcqcsjdec.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gvrdqvcem.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqlojysuk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gepirygtl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gfkbzmikh.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gksvrbeaw.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/glwtpieoe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gfxzaizuv.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gcoirmmbd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/giwpbgfas.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gchtbegla.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/grrtfehvs.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gncgjucxu.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gehbtfwba.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gsqkdvvru.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gfemoelbj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmaolaxcd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/ggcphsgqx.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gvygtkygl.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gvwlnlhwy.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gxvdbbmhw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gylmulgry.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gowgslrqq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwvqrniqg.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gvvsptuyr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gxhieygmm.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/ggftnpgop.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gjdoyuhwt.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gtcsdtegb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gyklyocmi.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/geernxfga.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gescgldxt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gjsibosav.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gvapdiwur.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gnvtbjppq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gffznjygx.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/glfadloio.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpmvaomak.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gytlxbplf.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gaetzhoxa.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ghlotdnky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gbqjkgkfg.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gqeovbkby.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gtfhoxpxc.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/geecwceow.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/grhzduxgu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggvnrrmce.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gfyfalbqf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gbobvypoq.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gqbxhbbal.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/ghygcxhwr.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/glukasazi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/grjyatziy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/glyouqknj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gugbscrth.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gzleqdjnx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkfyaisvd.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/ginmmfawc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gvvivmroh.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gifggaaly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gdfnbfjob.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gyubmqsiy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gfbnlqptq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gypdcufrk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gybpiehih.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gdweimvkf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ggjbgwbox.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/ggzlcipfh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gfmuyrtvq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gxffjyuvp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/grzcyrtiy.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gmemakmnt.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gplakbnlv.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gstftgxjf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gapfhdzdy.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gvbvcnaen.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/glitiwfav.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gkopyvdov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gqpinkynw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gkfcojrkj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/ghwduqkxx.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtomianww.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gvqplfjhh.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gurusplge.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gqkwsgmaz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/geswwgtpy.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gxoidihdo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghbbtzhmj.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gnggutuym.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gdxrbjjux.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gddwwdipr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gxtcmcvgs.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/grzencduy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/ggrlyhzyi.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gsntabkbk.sHtML


<!-- 参考信息 -->