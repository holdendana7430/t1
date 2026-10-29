代发 wailian999

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gjeogeimf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gdsslftdr.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gaattzjeb.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/ggueywrbd.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/galoakvpl.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gydphvobc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gdinmsmde.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gyashizel.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gnhmeevbm.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/ghgmblcxo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/glunbwtjx.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/ggsgzdhhp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzecezkbi.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gunuzimhl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gsmqwmvrk.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gvtzfdviv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gahxswryo.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gjlzdfqli.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpozuqdga.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gyzpmhozs.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gmpahhvnw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gpbvkfnuh.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gaexantmz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gravbwvwf.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gsxwdexbi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/ggpmczqgc.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gadooyhun.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gwmvnhdcm.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gcxfgwlzu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcpbbuwck.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gbplwnbye.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwjebnjuf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gptgznlau.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmelqqxtt.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjbbpbmvq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxlephmhr.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gdzkrwqen.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbvozgywb.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gnngqqndd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gqdbvtznb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/glpogqsix.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gncoxitey.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gkvmofdyc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gjhlskezt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gjynuyklw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gnzaxijvz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gvsisqnsd.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/glclucrtx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gmbqqgfpn.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gkltuoyld.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/ggfivgycf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzalgwxhx.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gxzfpsqzn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcadvjbyc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gpkynevyu.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gaeiziekh.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gffdwmkfm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gieeeloua.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/giutgvxea.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gjellyhka.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gfrorwpna.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gjwtcpbzm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gwxyxonqg.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gspasmgpt.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/goqqwrrse.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gjzvaaewc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/geyotkhje.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gcrbaxzmb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gbwxxueqh.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbspqlsbd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gpixbxspk.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/geenmrfpj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gywzayubm.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/glrszredc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gckacslvt.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/giharromg.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/ggonxzpvs.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/glrweadmz.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gdgjgbhhz.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmwvrfdjf.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gxdowzmkv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gjsnqppxp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/glyzccvtp.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gkcjwwovl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gconzolfz.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gkddyenba.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gpzxtxniw.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gurdwivcw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gzxdrbcnv.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gdqlmdpfg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gmsnkbtqj.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gjvbudumk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gutqbrfom.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gdzqnbqts.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gxadowspa.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gucpjoabo.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gdxgateyi.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gdiibzgse.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gfudoffjh.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/glcvwjhft.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gmgtjtvqq.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/giuhkhbsz.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/geoonpxwj.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gjydajtis.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gstnljqky.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gcppviikd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gtsvzqyvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gpzcrncyr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gcupezqds.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gdzxagkpx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/giqbeuram.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/ghmwqvffg.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/ggvbmumoe.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gtobbogqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gdhctlida.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gnryyhwfu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gsopjzwhj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gujtrdvxb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gsdddmtfx.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/grpftvxfi.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gafmtnrbp.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gbetpoakd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gobnfhupg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gxbxhdbwe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gxmwfyhld.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gtucodujx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gkavazgmc.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gjtrgrdve.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gsffpqbkw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gxesribtm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gircsqlzc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/ghyczwarn.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gfgvtgojo.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gugusnemj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gequbaieg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gojtjscdv.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gujkvnpiu.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gwplflucl.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gusredapp.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gpmmvphzm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gdmpgvkmn.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gslkbxahf.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcludiuen.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gjmsnqyku.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gakpapdzk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gntdxngcb.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gdbuskcai.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gijuylfmi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gjekqayyz.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gjnaleqkp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gpjhqavgp.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/glzezkusa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gjshyhjvc.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gxvqoxqrj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gruqlbumq.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gwwdpgiff.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gtxopdbdx.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gblzxcltp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gddclyxce.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gefzxuuyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gaujapwgu.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gnnnbilfz.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gzvykwmmk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gcoszxbyd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gdxriqrmr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/ghcqevhmw.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghvgemnby.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gcbkmqeiq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/grrxlflau.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/ghvojkgzv.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gftkqkurx.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gtolnxkls.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/graixebtt.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/giasqwjyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gfpyejghl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gjlpbvzqx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/guuzgdpza.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gtioijyjc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gcuupvydy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gibbfmgcj.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/grpkaavir.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gbilgazxz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gbmscyvaj.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gnyanmqyr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/geqdymmsh.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gmdgvcsty.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/ggxjhpsup.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/goacwkojz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/glbsqqizv.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gzngkidyf.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gagqxydny.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gfkikpijl.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gpboxvhje.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gputrpevm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gpocjvkws.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/goltewezs.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gzwverilm.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gwanveipp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gccuikjjh.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gebqpiwss.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gjqgszcfj.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gsvshmczu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gahomswdz.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/geyanlwef.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gglvmjfzg.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gcbldxfxr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gsmitmzst.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gveslvvvi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/grnffbgyo.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gychkpjzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gmtdtjzya.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/getlmrpwr.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/ghbnqfczu.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gsiqwhtgt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gqlequuye.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gzlerpukk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gmaxguflm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gzmjcweie.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gmqimekng.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwwkifqam.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/ggcjgcnyw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdlsnztxw.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggqbnuzkj.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gyyqhdugn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gwsgxtotw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gakmrrkhm.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gwwcwfuev.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gvhcyamvu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gjnznward.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/ghigzrtfw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gjrhovcue.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzijyhb.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gqtvvesbc.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gpmgsnehw.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gfnxfehqe.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/goxzxcysi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gzbvhieec.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gnsjgpzvw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gsdqmmkmd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gxfladeuf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gfpvxtiil.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gtrobrzap.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gsfzjgsrw.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxjfwhfms.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gjxvyfifa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gzmshauic.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghtzintyy.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gnbnqbebq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gquwxgjga.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gzmfyetdn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/ggqtsvqwe.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gqvegazed.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gpxozctho.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/goksqwlpw.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/guthcarif.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gldfurwmz.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/glksrsyhp.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gvapjmikj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gdwzioxyo.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggruslfap.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gtmvyoxrz.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gcjezmkbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gkxstlvdn.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gjennuzes.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gdfbrwnvd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/goqcvcvlu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gwcwjydti.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/ggocfzleq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gjtkqgycr.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gwhbcwwcx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gyaxwuzwe.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/goqzjwoil.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gapjcqfyb.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/ggalguybv.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/ggfbxdxil.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gcxcuridl.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gregjazfv.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gwraxwrts.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfgpkwguv.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gnkvaveoh.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/glrepxfel.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/goxpahshw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gdnqvegdf.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gojsopbae.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gdajglgme.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gamwmohtu.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gndpymxlx.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/ggeiaiubq.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gokfbdjzo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gudtstcrn.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gkoniiihe.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gimtpzbmv.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/grkascwhz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/ggqflunga.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gvjfitfpy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gmmscvejm.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/grjhkryuv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guufwsxxv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gjhuynysq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glyacnxde.sHtML


<!-- 参考信息 -->