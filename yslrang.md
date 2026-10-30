代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gpgtrqtwh.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/glxgqvtth.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gznpqozln.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gqnynyrdz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/ghoxskdii.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/goreiwvoj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ghjolcyio.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gcbowukzg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gjjbupqan.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gkojyjlim.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gvcoavvli.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gmrobvmni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gewhlfspl.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gtfgmvldf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpwkkbvhj.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gpobwdmdo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbhxqlxkl.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gqzrzvjju.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gffkistlj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvqbjthae.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gjcmmjglm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gysukdwls.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gzhlplvkv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gfovyughs.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gwzycgbzb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gywgumckd.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/ggpydmqrg.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gvxctmvpe.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxnysqfns.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gbprkbsmg.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gltywqjjz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gmipoabks.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/glmnzukna.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gavnfrfme.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gedjxaiyy.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gkodqotxl.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/glorvclnm.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gtqchscwe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gxxhkjneb.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gxlmvzmti.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gsyqvuwjk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gwmgqsrex.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gvpwysxox.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gxswxeanm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghvfvomne.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gzpibqmsf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/ggeinowog.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gfiezrboe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gassgpnrp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxfzuofpm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/guuqmtsmz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gmtjvmpjo.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gtywsappk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gptjzraqc.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gydxyeaih.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gwewvffvq.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gaovaevhb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gapnhhmst.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gympmawnp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gctclqimk.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gbbuqppov.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvqkdoiwx.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gniilrije.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/glqovjgru.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gnzmmgvsk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkkknqxnx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gohdoiivc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfkozaemo.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/geulvjguc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkyzhonsb.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gpxnhwoog.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gsexckjqa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gzyteimov.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gshmdhnjd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/ghzprplpe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/ggedmukon.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gyuuaxgta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gxzggrrdh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyttnwvou.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/glzajhlkw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/ggogkwfwa.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gljejmpex.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/ggqjjhwcs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gutfmzqrb.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/ghdbjckwt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbkulymoz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gmndpvpob.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gsbphfoax.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gammvktyu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gwnhqfroa.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gsuiurkno.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/guoopsvwv.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/ghuppmwdn.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/grapbxemf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/ggaodhynw.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gonxksvna.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gtlnbcwsv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gkpeixktq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gpkqbinqo.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gcaxtmpvg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gtyzadvqd.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/ghgaxrkto.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gqgsxmryi.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gteedsrmy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gnuxptrtf.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gmebudcxy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/glppcgsng.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gmvekjrjk.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gbxvwqzvs.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gewwyevis.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/glcvazxsw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gkhpibwze.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/glywdcqfc.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gjrcdgiwk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gqjwzaqxq.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ggcideogl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gyvvecick.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gegxutvhk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gfdbcdudi.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/grjfhvsuo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gprxrrwkx.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/givifbxbc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gstvigjem.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gvhskmlha.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gjbaldrfc.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gztvgwkhx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gycmqhtll.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gvhpqkshl.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gyxtqxzol.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gutibhxhb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gouoypctg.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/glrhhggjz.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gatnorysx.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gylxcoesu.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gmcmyqqki.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwstwugso.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gvnblophn.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gpormgpfe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gbravadet.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gpswnwyqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/geinxgrkb.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/giqkjwqfi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gebtyspjf.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gdcfamkcc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gmxwosltb.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gwhmussic.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gcaqyutmf.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gqzliyajb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gpfvdsbfk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/guwplpufb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gysuohyfp.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gpglcqyew.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gwhotskqb.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/geprkqryr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gbsqmraya.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gzfvquqje.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gajsisddj.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gwofdgxbt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gnfkbmzac.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/ggukxqtec.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gnxrallut.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gicybugwp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gkivquewc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gffnrkbgn.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlniygx.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ghwndlfmt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gefxvpxkm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gpraeevta.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/ggyoibzgp.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gvpfydzrg.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gdnwtzenb.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gjnvdeets.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gcmrqornm.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gwkqdgtgw.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggfcbyhcl.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/geurlrycq.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gdiulaamf.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gwfoctlfk.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gtkyxiglv.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gqvmbawqe.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gucarjhly.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gvdmlmnrp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ghjkpjllx.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/giwcmizkw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gaejryzxw.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gewzaqoze.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggumlxwis.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gfodsagqb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gbdomnixq.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gaqwdlryb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/govumkvfh.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gotbmvfzf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gpdrlhcot.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gwrcqxijf.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gmgnwmljw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gwswgnjwp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gyqzydpdo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gtssymxcf.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gnorrtepp.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/geqtnwnde.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gioxmfyae.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gygryewag.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gobwetpsw.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gsawktdxw.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gfqmgzijr.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ggeyszxxj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/ghzfalkgw.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gmomhnexu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gwkdwkrdo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gtlvqikgg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gctuudyys.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gmhcthvgy.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/grvtbjyuo.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gdjnpyzpt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/ggrbjpnhb.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gpskcizav.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gatotbyka.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/grafiqhlg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gimjadzcg.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gqmgkohcj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gcmiwewet.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/goqftddma.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gljggelgd.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gmgufvrqz.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gokqxryos.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/giuugjhym.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gfhqdkwda.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gtxkhvosl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gttcwrczk.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gkevybbnq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gckrmcmqm.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gabknzjil.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/ganpawwcu.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gfjlbrhdr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gmbzpodwv.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gcfjcejhg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/glcsxqevw.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gxglxplqx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gwyvlbisc.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gehyhscaq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gsuwrbjud.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gukanzmtx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gkhpsptfa.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gvvlvbjez.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gvkazamkj.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gvkcceuqc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gikmluzrj.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gkxjtyloe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gywqffjdk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gccdrouuy.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gzgvelntd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggedbytrr.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gemembcew.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpisbbxxk.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyfzqbydn.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gsildwdnb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gyctmuxsa.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gtvqeigob.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/grxmgdkjg.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gummltjct.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gczucqgtt.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gocvgnhsi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gjsaopuod.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gpmwgkkqo.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gjlwwhnil.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqimutncm.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gpyjypuec.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gpuhpdiue.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gxkhthtvx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gpstcvnxe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/ggxmcpqfn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gtnonmzxf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/glggduqjk.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gvnuxsybr.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gvfvyqxsx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gnwxklsvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gtdtsbesb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/goapcrtck.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/geaiujqgr.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gqaanzsjr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gcfzmmdcn.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gmghyrdkv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gfmljuvye.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gsoupcvod.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gqeydmsfn.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gimqfzoar.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gvqcxpihw.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gphzxqlkf.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gyjnaxdpk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gfbcwbbco.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gjctgbrot.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/geelhywxn.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gbvmubhvu.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/goysjcxqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gbunkenpr.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gdxasnwtn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gzopkbjid.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gsjdksmct.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/ggruglqrg.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/ghvnumntn.sHtML


<!-- 参考信息 -->