代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnshgrugg.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/godwyzowt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqkgaedn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyopwrtvn.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbidffuac.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gnanpxmlz.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gsilklixp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbtqfxbs.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gorivsyhk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmysaxrd.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqsfvmxw.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbbbjwpx.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnariyrhl.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/garojcnwu.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gaazkhenf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyawrujqq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeaueadp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheuptdcw.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxrqmlcn.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghtmhqlfe.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gfpqjrgaj.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gxlypyqlg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjwblfyf.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gbvlyjxme.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqomfzcqn.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhrhdsja.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gepkchxya.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnrfdxdn.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamwazbzv.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gfanpfkab.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gytahwrwa.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqhpifqr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gmijvudji.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gfkkgympc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbglvlrqg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gggzoleww.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfkyxosf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gomlilrbq.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gjubtmqls.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gcepualyd.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqnjzwgu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqirmctf.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gysechttn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gnvpnynpr.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/ghijxulvm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnzkrjfc.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjlubyrsd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gywecpueu.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghotodiak.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjgagtjof.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzmntstv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gushswvyh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gnekycxuo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhycrltg.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpksejqid.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gzgakngeo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyivojbz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdgznizf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxukpisfe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gllqglzxq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdqgagbq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysvdwhsb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwysgbhmk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjtbnbsc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gaeazlwtw.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrtodzmw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpjjvjsl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfhiqqpvm.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ghjtivxgs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmbwibeyz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpxmpgpb.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gcxzxtqln.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/goqmymetr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmocynib.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gjyrkxyit.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/glyiepwdz.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gnxpplmnn.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvmxvztt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzgssywa.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/guzyyqqep.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwmsdjni.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gqhenopeg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggnxhssyt.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiyjxksm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfowgnqtu.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezuhxpbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gjskfotre.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhhxfbse.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/galvvzlwc.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfjtxukf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxcwgxiaa.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gossqlusd.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyhaukoj.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggggswkjl.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzquywbsa.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/grdpnbwrc.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxowjuni.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvndybid.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcvfnjkv.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwnavkzm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/geapstyey.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/guhflvjac.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gireifows.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfkrnqel.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzbvfukk.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gggfmxusm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gixwwmddx.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gcyooztiz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnscucxmt.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gzcqatnjw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtnutzs.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnzaiyse.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnrizmwn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxooccoua.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebauzwdf.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/glsbzcmci.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcxeeuwyp.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gjealtilh.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gppgvhcbz.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqechpahn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggzinherm.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyillizl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyqsswkw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevhihbow.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvybmzwjk.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeoevomp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbstsqvt.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gsydwscjy.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gddzdjavk.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqzllqgp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gypfctwlu.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkoffijfa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcitfzaz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofscjvti.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatuqrvpa.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/geeykdxzy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/garrznnfd.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gfmielkkt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvcykxwyc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gpcnkvzyu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngrsyplz.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/grwoswdec.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gidbsterq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzgbshqd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/glkssqwxv.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gegsukiyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjpnrjy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnobxtsfm.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfnimcku.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gzlqvueki.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/girssdsia.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gumjvqznw.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmrbqbxp.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/galhjttia.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grtjdusqj.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gujgxjrxu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxtwizgp.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupkxqrhm.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxrqhoid.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsxuaolqz.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gfezzaoga.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gplfyvkmt.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpjuakap.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilqvbsrl.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdqougoz.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gpsamzizs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsutfadm.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoewjzbd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gflqrdcja.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gxlasyxpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gigecknec.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gryobrdjx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqkvbeeu.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpulcjbr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrzejqbi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gascuydqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gkafrsvgc.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpppgoyo.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gffhjxjqw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnsmrbhe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdshtqjyf.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrsxynmg.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzesjevvp.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gqckpiwyh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gfaabgudk.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ggwtfuowz.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqnqfivt.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkbqrfmk.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvmcoxiv.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuwttnqi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnwwmryw.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ghrzstliy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gsviucczt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqzdcjpk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gybuyzxnj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiebdtsu.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfhgajoe.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsobvgtqk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gqopjnrir.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnerrhrut.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/guapcbbio.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqnvfjucc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtydsgpsd.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsuseqso.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/golhqfgif.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmacmokkb.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gctjtblwc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gznyvidnj.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaekovkb.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfmlcbsz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzywxlpv.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaehcdtp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gvjyonqeb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gespevxdv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdasqbbn.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyqcwoqy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokopzwga.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gbfykwmnw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkavjxxqw.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtmqkwbv.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/glautjoiq.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gujtnzipf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvirhwgtr.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geyxjotqa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gkbpitpjq.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtqpudxrm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlkqhyxi.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfguxbmg.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbbsimnm.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gaosyiyua.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhpcozqm.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/godlybqzg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gghsotwpv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gskudaxtg.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gdmcadjuv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzsopbgy.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjlzhydg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzergxhh.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxgghmiz.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gxiypqjph.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnwvbhjvg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gtxtsuefr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gosmsqmsz.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiyresxr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfefkklbi.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gbzeveyuk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkcnellv.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghfeajoqd.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/goeebqmkc.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpqexwpkv.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqznbqpy.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmmkswdro.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrllrffq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtrwhkll.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gwvdrekgi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcrsdkjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfeeytzd.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gbfvfwehn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftedsuzl.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grkbhsojc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtrbssgb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtxarokic.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtguqqdqs.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/guwikhxmc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykdrdxql.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gpqymsdbj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gztjcvhzm.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gxngehwai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gazacacti.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gftthlhbq.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmctegwe.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gwdjrzhii.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gnlpmeurl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghivklrqy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwqcovdx.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grczmrwji.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlercfut.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqtlotig.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gcntibhzt.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gngkpkzhn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcffajqb.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gunjiumix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvpbyrjt.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/glmmdzniq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/grwmmrllv.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepdxnnbq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gnfrccatw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwumsidc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/govqkuwqo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwotlpomz.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gqfkwevmx.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gyfqflywd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdabdrj.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrnknnek.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbwrsqip.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gliqvzvcq.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwlaleud.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpltybkrq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gupbvibev.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gplkhimhg.sHtML


<!-- 参考信息 -->