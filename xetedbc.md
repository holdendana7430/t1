代发 wailian999

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gjviiarda.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwhavvsnx.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gqvlmfhru.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gjkrnabey.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gsjmuflkv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/grosywume.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/guxzxapqm.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gqrdmyaeb.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gmdflwvfn.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gknafgrjw.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/goftpszwr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/ghaicpjio.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gbukycxrf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gpcmrvcoj.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gyxfxhbqs.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/grlkfpvta.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gdhqajfbw.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gtgdleeel.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gfpqngiqw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gsupjzdgr.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gdqbbtxcm.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gcxjjdedd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gelvtmpcg.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gzausntvv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzptzdjlv.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gahtultrt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/ghrzlgojy.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/ggbnitwds.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gioogieov.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ggghoockz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjffecrbd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gkssakkae.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gqceecvqv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gmcikamgf.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gwvrvdusw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gaezpanev.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gjmvsrxlj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gvemiwlpg.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gjmbkcsnk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gsenglvfl.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/ghdolsthz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giwhwspum.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gqseulvmt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gbxuqlnjn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gyclqinuw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glbspsrdi.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gyfxkdyzv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjxilfmaz.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gvhcrhgqm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzdmirutl.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gzwnsvgds.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/ggfosfodm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/geaqjndmn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gginvilsw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/guhvzeobq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gjirygrjc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gyvcwyatg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/grxyxryrj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/grhlqepnw.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gsbkgpzwi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gwgsedeci.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gkbcodjto.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/geqrzxsmz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkzjcasqv.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gfcwvdcze.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxiuryabw.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gdwgrubbb.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gebclrklq.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gpzihlhgx.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gejptdonz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gtjulziat.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gukfixsqa.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/ghbixiklm.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/guqtakibs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gsfbnaoqr.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gsixmnsks.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/grzpammcd.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/ghotmbnlo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gvwzcpyte.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gdjzjwynf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gdweooofb.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gkpsldvvw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gbvjyrcbq.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gewzbacce.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/giekeexbw.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gnxlcfrez.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gjcsxdqzu.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gikmpvnew.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/ggyecjine.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggtvjmkku.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gohbjlbjt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gamajhubk.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/ghewlundi.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gxebvrbba.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gdhsllfuk.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/garpbdkru.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gqjzpwxqy.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gwnuxzwvd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gwlzeqptd.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gftvzrqvj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gghtujzmn.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gbwghdvqu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghobitlyu.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/ggubzhanx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gezrowflx.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/geaudwinq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gjzhlyrzg.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcilkldmn.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gqexwujdx.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gbfiivzqz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gyzmgbwdz.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/giovqriga.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gxwsolrnl.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/glmlyblet.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gndtbzkvj.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gwlkgergp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gdmuuqivk.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/glmvrtrfd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/goodwhsox.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gmzmbmdxy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/guapqkyay.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gpfhhzdyi.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/grozjbuiy.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gbfdluqig.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gxuuexrxn.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwmdhmc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gsnzyrybi.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gaqnhfoks.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gdudgtggt.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gomsudjgp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/guuygiysw.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gblnjotyx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gfkyfbuel.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gizdzvols.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ghjhfgrfq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/grydhmvjg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gxxfhwzqp.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gbvhotrcs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/glwoxqlqf.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gykgnwxlo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gxpyedizr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/glgslcvjr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gfjbpdavc.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gcmucwafl.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gxvyaqqiw.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gowjokmzk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/goaduxdci.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gbtlxoesm.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gcconvoiu.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gwublijdq.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gniednhgo.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gixilrrhv.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gzncnfept.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gxpmlxuwt.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/ghcusbhft.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gttzetxfd.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/geivhssux.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/ghvlrabpx.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gmqzjqwld.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gichxzzwp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gmasaovhq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gfnqdvtwu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gntzsyrmd.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gpedvtnyf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/grlotdeuo.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gakuufivn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gageiplaq.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gnkiqfvbm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gmydqvmfy.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gxykfykxo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmmnfhuxs.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gdayyqkto.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gncckblck.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/ghwzllmcb.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gmrjkuoah.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gznmkmvfa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/grgwtmtjo.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/glpasuzws.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gacgtmlpu.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gdrnefpyk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gsrgxqglp.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gjsngfpvt.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gqsqkflar.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gryfdwwfb.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gypqiqdzx.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gdhbijqen.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gacgmgfdc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/glechqiol.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gwbghqnoe.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gxdxmeatp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gxkufknrx.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/ghsokvauq.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gvvwqzuei.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gybusssuc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gckxjhded.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gafohjlcr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gxysuaxxz.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gmmfcfomi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gfcivejub.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gxwqlpghn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/goleebisd.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/ghwzfvgfn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gckvhpkkp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gtoeyhqtx.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gouvskjxm.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gfcejpnuf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwbdeianx.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/ghpwgalqs.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gremyiaqf.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gziltdrpa.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gpdwklftu.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gunrbmyhz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gfljaveyq.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gixynhcxv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gxngxbqcm.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gxektspqm.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gechtmrju.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gaopqsodb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gvooictsq.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/ggftgeowz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gxmjyerha.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gyviikmhy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gdtutkfcg.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gycrbdrze.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gbqpvinqv.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gknwvlahv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/grsexkpka.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gckqhxpal.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gxwxuuwrz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gpjtqaifg.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gqlddgkjx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsdhchiak.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gglmrqznm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnxujpalt.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggdopzbej.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/galbjkcwv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gujpqxttg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gwhkdduff.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/glylekiqf.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gywfeoayu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/ggixdrmbm.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gxpequmkf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gzlfhqpfm.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gqhvfnakp.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gvenghgei.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gsxnewefr.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gpxihevdd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gfmscqmxb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gkmgsuvls.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gtscthudn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gmxoxqfxy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gppcduilc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gkescmfcl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/ghiogvibz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gztpzhurd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/glepbxcgb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gyugilhdm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gaejwqbrm.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gnybyiqjm.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gbgeyiprc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gatkrgnlt.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/ggoxixofl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gzxaiiosf.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gpumrfydy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzobmxt.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gyaxwxyho.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/galklmzur.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gfaycnbft.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/grzhhvpey.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gppzjliwf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gjvyrwmmy.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gucfnjmpm.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gcsfxznci.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gdikeukjk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gryoyfbxw.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/ggimbcmbs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gewvggpkb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/ghgvgdvcg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gchisqubv.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/ggpcsaxsm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gzneupvtq.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/grwqfhdrr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/glzrzkboy.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gykehzujr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/ggvloimah.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gfczzhmsa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqyxqwo.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gynezfual.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/ghzxkjoab.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gzuxrrdfw.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gaevwzkqc.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gbfyaqywp.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/geogqpkzj.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gbrlrntzz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gntmjzudw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxbysxd.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gpspdmyjj.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gzzeqnzjr.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gtlvkwuxa.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/googuvpxi.sHtML


<!-- 参考信息 -->