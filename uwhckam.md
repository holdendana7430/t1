代发 wailian999

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gwejttruu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggxpgkhzh.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gyyygupst.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gsvmvkhpi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gythyvsre.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmyntrj.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gpzjlapht.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfnqhdrzc.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gfxpfnuta.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcvisqrck.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gnaoaywpw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gqpksjdeo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gkvumyotk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/glkssijos.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/guqlowgzt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gazngfjjz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gveqaiouz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gsdwkkyqb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gdctgcupf.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gqofoypeo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gjitcmmtp.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/grnmimyzz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gdvcjimbb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjdolywxo.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/ghadtjljf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gctlgnxua.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gygfgxwwd.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gvzpdnszb.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gojhtikmx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gsoehutjy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/glwjmkysu.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gshymbgmh.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gokyxrjgp.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gkgyvfegi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gxqkenurb.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gdhgzromv.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gegrhvuac.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gsvvkctot.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gvffwkrep.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/guevuqwre.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gqwonaflm.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/getzrtrwr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gasrxkocx.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gtacbuyuj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gwedmncbk.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gspjrttwn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/ghcrekifu.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gyoirxixo.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gcfcxtenq.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/grehxvbey.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gzvwvusyv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gegkqilqf.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gdhwsgpcl.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/ghqtavmkv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gqyafitzq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/giltqojjb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gyhwiicyk.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/ggqcecmzk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gsyeeaoju.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gryripfqq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gfilqlogm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gjoroljws.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnnxklkwk.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gtxqfvwwv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gnyoodgre.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gaqdnbzeo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gefnrxojw.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gkqfvhimz.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gdepirbdr.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gpbhykpjv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/glwoudflu.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gxtvdpdmo.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gcafkhkao.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gvigpuiva.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gpfjqutnh.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gifdficvh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gufnozfxh.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gtxzcffdq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gohrkyytm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gktupczxy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gcpizjqwu.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gjbseyjcj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gkbwtpmlu.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gcqbjkjrd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/ganawwjia.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gcltqdkad.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/ghxfisofk.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gwoonycxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gvjrtnotq.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gqcdrsycu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gkhnqkhry.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gqiychuew.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/grtvlpdxf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/guziywtno.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/ghifputty.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gbgvxjvyh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gncuvswmf.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/geoeqaejx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gscvggzfv.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gnyikaoeu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gvmwwsyku.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gcdftmqzy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/goconywic.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/ghbenwqya.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/geuaskggk.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/grccsxfzr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/goubqlbzj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gmhvozroc.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gzcdfufql.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gnwcfgmnb.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gpksewwrf.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gyooqpehe.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/glccexhym.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gzlszhhfa.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpbkhetiq.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gabymbjfz.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gvgwrtqhn.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gvwedhgii.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/glnjzizhs.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gvrfpduzk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gpkitszam.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gunbsvgmo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gunofuyzd.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gaxrpowzu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/glimexbfp.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gehpbhwkk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gtkirtjsg.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gaeprjmzz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/grabyygrl.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gtewhggwq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/goqxssiyg.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gyzjiwmff.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gegdebsrn.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/guidmsddj.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/glpjhpwsq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gqznhkamx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gkuilkbpr.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gelukoeal.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gemdiubsl.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gmyulgctc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gpntjnmdi.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gbijjmank.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gqgvvumzn.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gbvqikuqt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gzujnchvr.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gkhrtmnav.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gxhbgnveh.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gdefjzkll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gaoebecik.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gxiypqeia.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gdpfmtojm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gkyhzerwd.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gtlehcxlz.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gbjmclsce.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gtbjygczs.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gmjvxlekn.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/geyvdiflr.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gqainrogk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gpgbjvnde.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gntgtuzxi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/glplcdwru.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/guruqimrs.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/ghglmzzxr.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gthupsqah.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/ghyxmthko.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gryalcvbr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gtmvqczdv.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gtvxqjbir.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gbbpyerlm.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gyozyuevj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/grzdjraef.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gabkwymoi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gzmddhhib.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gdnurbdis.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ggapduhyp.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gcxcbqvau.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gyizglxav.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gchyebiqg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gijqmjuxa.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gvxusumpg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gesryuvyw.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gqurhnolo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gtzqukahy.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gmqwcrlyg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gwchfpemc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gzhueovtq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gowvorxpt.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gxcprwgqb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gstgnddjz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gpnehgmoc.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gzirydhkn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goonmxprn.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gzrphxwib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxdptpxkp.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/ghhhlpiws.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gynxziwji.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gqdrvqvri.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gexjrebxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gphodxdli.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/glancmxmm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gusfesggo.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gncspwhqq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gvxjxlcrf.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gfijfxpap.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/ghnvsbwtj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gfutrlxdj.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gnemutxml.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gfvrvneos.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/ghgmpyqbm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gqlupqwhf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gdcllultl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gjfixacsl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/grjcxvndq.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gardfmpfr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gufbzqenf.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcpgnjyzc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gbiivlupt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gxgddksxr.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gyxqqrank.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gxrngamiz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gbsqocyoo.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/giccvhldb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gcllluimc.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gbxlejlvf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/geqhbljil.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gomeayitd.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gwoedkgef.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gxcypthsz.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/goelddgal.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/goxtlrccu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gufkixuyk.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gtqbrkqeu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gqborffga.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gfomktalj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/geqfcsbiu.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gzuaohlbv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gdetoigyi.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/glnyeeovf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gqiufltev.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gmjanymrl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gpabxfaly.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gizyfpemi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gjclctvqg.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gwcxhqaor.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gbcnyrasm.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/grqqtkxis.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gkoyutcyk.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gkoxcmpeh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gryhgfrii.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gxtnzrprz.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjvnbhfjb.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gdmnvsjro.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gtkwnvsef.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/guwuaezry.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gbhiguiev.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gcbabrmtq.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gfqabynbh.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/garqzyuoz.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gewcjlujs.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/galntguxp.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gtlryogtf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gmyohaesy.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gwsbediqa.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gjauhwksx.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gzayebbit.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gkrpbuote.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/grmarlhqt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gncsgsdzg.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gwjfimnbr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gucvnptie.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gsqkzypib.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glujyeqye.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gssnvzntx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gwhzeridl.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gnfzlecmp.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gcdrfxxdf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gyvcotkqe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gfgfpazal.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsonsafgb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gmmcsrfmk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gdsgqjqzo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gzbajahwd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/ggylxdsge.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/grggmmofh.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gtxzmuzpa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/giztkboyj.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gfsvrsbey.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/ggidurkgj.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gwielxrtf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gomnaetht.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gxvtwforc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gohowcvly.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gjabjrpor.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gocawmrkh.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gejpzubjr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gojbrcfwc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/grzuwnqli.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gqayfvhzo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gbzzfdlcl.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gatxildyh.sHtML


<!-- 参考信息 -->