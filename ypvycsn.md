代发 wailian999

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gttotmsap.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/geivhapfr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gaeqcyhfs.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gmtvwfolm.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/glhmqzjwd.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gxmynbeyg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gvxjgyqgb.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gttvpzgur.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdrbjabrq.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gbnkryvmx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gsoxbdptl.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/giltuvuks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/goheaquuj.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gkynsadru.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbxqmqzin.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gmbqcaylo.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gqsmdsgsj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gkfabaypg.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/guejnfeje.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/glfrklnbt.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjkrzxflp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gszgriwmv.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ggshhyxyo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gqyuiyaaw.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/ggwdxeuaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gykhhqyrh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gzmwgwltu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/goqwhissv.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gvqgnafoa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnlqdjwrd.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gxdrduizs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gowqjnhxu.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gkzfnsdva.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxndjawdv.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gcxgzltjl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gylsknyrz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gyroaqlfs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/grrnosgms.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/grronnbus.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gujoenmxq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gjpwqbgar.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/ghgxromma.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbwsplnxu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gftftuqky.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gidufsepd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gptemmbgm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gelrutjft.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gevhakdto.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gjdibvyds.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmfziackp.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gnugxmgxa.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gkqvetzpp.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/geiaekaob.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gytvjsvjm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/ghwxiyrcu.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gwywjevhr.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/ggffewtbu.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gkrdcpbsz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gpxfvufmb.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gealfhxfc.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gwfxzjnhh.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gpsmwctxv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gllcgnqwx.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gowjeilnf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gstcsxvus.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gqflmolyj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gvtrujzow.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/giemybvqi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gohxiifvn.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gujiogcsm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gitritnil.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gbrtmqxdv.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/ggkxblcqx.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gyiexslji.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gevxljavc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/glziaawoa.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gralczgpe.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gxyccvasz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/ggzvfmelw.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/glvhecjqm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gjpesmxzk.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gmukyanjh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ggfqjmqyy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/givzrxkwv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnfdvijzk.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gunlnbftw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gwagdpknt.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gwbfwbjgx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gajorgcyy.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gngbiqmzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gwnrwlghu.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gjhufscye.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gfmratezt.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gltmjepzr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gjoklhoas.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gszbddsaw.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gjtolndqt.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gxtxpigkf.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gtnksuylu.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gvddizuaw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gnebtzsva.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gkarlcfny.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gipzeovis.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gmfxrselm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gjknjnale.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gfckphdrp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/givezpamf.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/ghtxrrxhy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/guboggoxq.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gqryiclyj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gvwpdswca.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gresrtaqu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gbimwbvxv.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gafulcvfb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gpenuylom.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gjeyurydh.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/ghmbgqqul.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gujikctnv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gdxillphd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gbbmkpdeo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gawafdiyz.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gwxffuvut.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gdfoxwkmc.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gyabmyofx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gkjnvtgls.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/grmnjhvxz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gfxdvydmf.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gjsspmrzp.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/guubnzaei.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gymtewtin.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gmptzhoys.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gmrxqvglj.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gvqxoashb.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gcvqzcbnd.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gwgbhrgeh.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gvfbxviqh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gxmfpntse.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/geuybyqbf.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfjayqeyl.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gmeyjfgtq.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/goozzohjv.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gwhtdzyrq.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gsxeuvyle.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/ghwbivnxf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gszchurch.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gjsliiufn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gtvwaenik.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtyllyfvu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkpkcjdmf.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gnignysgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gjtnfwxoh.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gjyurhbdf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gqjloocri.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gnnbyavrg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdweecmay.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gpjuosows.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gcpfmggtl.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gvlwgkklj.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gsxjtxspk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gdkyckcnv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gfbsxfvva.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gwbrojqtt.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyfncjycm.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gyjctmpbn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gomdhyvxu.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/ggdecnjec.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/giouuemkx.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gwupnoxoq.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gpteqtuxk.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gkkluoybx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gusxnhxph.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gbxcfjoga.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/ggecycsdy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gsvvebdml.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/galwcdklj.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gasmviwnd.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gaoftmpsr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gtrzwgsul.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gwnexwjgq.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gtjrgkldg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/ghvsyzdue.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/glsyzczre.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gnigaqlzg.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gmxyexoph.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gywxeakba.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gufldqpck.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gemaenhfe.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gjpdamydy.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gtiobdrph.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gcgjqjujl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gfaczjmun.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/grntkhmub.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/glktzeluf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/guombptsn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gwationki.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gvyxzmwte.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gjvxjkgxp.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gfagzylnt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gchshkjwz.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/giuracgcr.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gdqxbjnka.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/goauamybq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gugfyzctd.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gxxfcdnrw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gmgrteudk.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gkhayunxe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gciwwrntz.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gbyapimpa.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gfudaspxv.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/ghqzoonwk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/giepvgbjn.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/ghbshvepe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gtixfhakr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gooirikoo.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gdgcdxvny.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnydgaoul.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gkpdqsofc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqxtbpayg.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmyojqont.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gdullqzrp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gacgozbvm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gnhdwhsac.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gnqjyitwr.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/grutizyag.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gczvaokwm.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gjjcxrjja.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/goobvuvhr.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gxskxfvob.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gyclrffme.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmyjzmmdc.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/glgskqsyj.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/geyqrqrzo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gsfnkrdvn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gfxurydnv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gcozpdium.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gmqzwhckw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/ghppkymky.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gpbhdgxsx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gessjpncl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ghqycyuvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/glrzwiobg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gvihoqmxo.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/ggebdzust.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gozfhjmhx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gifozbaqp.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/ggsilslri.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/ganaraxmq.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gmbaeeypp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gfdnfuytb.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gxapguvzn.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/geusrldxw.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/ghflrzanp.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gjxeekasu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glyoqismf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gnmojgwny.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gclyifjzn.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gwgdpoywv.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/glpufyngj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gpgqjhnil.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gwpcstlif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gzrfpzprr.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gmaqgoorg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/grrabywfq.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gslelyyjh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gyrowhllg.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gtmgicykj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/grzgphnel.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gvjphatvp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/galwyamdl.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gutjjzmok.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gxrllkqsj.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gvnjpyjfh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gfmhzmzrc.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gjjtzmbbg.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gyubikyhj.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gewilapbm.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gvrrzoniq.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/glbaxsjse.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/glpltztgf.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/geujfhlbn.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gvoamxhez.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gtxcrcihc.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/grjrbxtqr.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/ggjguxahz.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gtxzjuhsf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gpmianlru.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gtpsyajkz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gohnrxfgo.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gaxkgizrx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gwftypylr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gyvngeuyr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gerfkrqvs.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gjwypcdnw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkmrwkgxd.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gxdvkupco.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfcuvdyfs.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/geodgxfpk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gfbwfcrei.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gzetkmhrf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gazggroei.sHtML


<!-- 参考信息 -->