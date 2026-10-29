代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gzvbsyude.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gmqiftgic.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gpgqpqnra.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gwppjvfxr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gqbivjdgo.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gvthsqset.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gplhotqwm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gtuqezlnk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gusshcswa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gvnzmzqqm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gyqyrrbsq.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gfmhanqzo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfppifbqn.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gzazcbfpz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpvuomk.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gezrxdlqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghetugbir.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/ghfgiojqb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gpjkuwpbh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gebaddlnh.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gphnyqbsr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghhudyhnf.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gzjtraitx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ggpkabqfn.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gcnrokofm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/geaqshini.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gekyyhyid.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gtvtgaqqn.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gxkqebdxf.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gthkrspco.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gvugdwuxr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gqrstlhui.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gqasrnrav.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gocacxrle.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/glnewncdv.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gsfyfmzlk.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gfxchfgoe.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gjwktacax.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gcxrdgamy.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gyzenmzfz.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gzaqpgqnf.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/giwhxnayt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnxujdiwo.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gxphkktxy.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkfujwprd.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gyqzfaeaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/grtmievxb.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gmzmztggl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/ghpdqxnau.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfhspiqix.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gectyaczp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/ggmbouari.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gvjjoswxm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gmnfzkznc.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/guvdhuxlz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gblwtttns.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gwkujmvqb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/ghtjspxwj.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gqrphpiki.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gejxjdrog.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gaocpwscw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcbznkqca.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gyhvtmrvq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gychptejs.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gumtdanvq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxnvrxbxs.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gvyepmeim.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqrlfnrjw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqmealn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glbdyjupi.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gnejvvdxz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/ghrpfqurq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gfvqjhmsn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gnsnlnuyx.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gneikgzdj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/ghbdpqjja.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gfewevpxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gjvshrkcs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gnsdqrlwp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gyntozoro.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gnwexfmqm.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gcepnpcox.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gobsydmxn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxbhyatgd.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gaemovxwe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkeddvpet.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gfsoiffdz.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/grazzvawk.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gtywfukay.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/garxlginj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/ghjvkobod.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gbncfbjgm.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gotexmbxv.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gzfspsadk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gnqvpimvw.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gigopsxms.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ggtxqmskf.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gqrgotigc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gaprpohhw.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gqydrhfub.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/guizdbock.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gpduowzmy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gzkufevut.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gerlafinq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gpnmndrcu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gmmwiealc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gxpcgjivj.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gfiuywjyl.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gxyjmtqhg.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gjwbuftaf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gkxrnwdhw.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/glwrltsfa.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gdtdcelrl.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/glebirfzx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gsvhbispe.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gowmgpcxs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/goaryyill.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gbgysydux.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gfkzltkrm.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glphfyxnm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gdknrozce.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gtqcpqbqv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gxcbljrap.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gizyocfie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gtrjghxqc.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gtzvuxycj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gnpiaccmo.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gmwciotpr.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gfadjcjsm.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gdawufdcw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gtenqkidb.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/guorzhfzg.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gaocifkqs.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gnrnmpshi.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gxdcgsbbd.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gqtwctyzq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gzgsqansk.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gfxdxylzp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpxedhwdy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gkhsbkdxs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/genngpdun.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/glahtlhhi.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gprvyxcqp.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gyymdndtp.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gvqezdklm.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/ggxjhnjrr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gmxamiqll.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnzktbazs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gnfwwkdmr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gmjxzfcda.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gxzzdqidq.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/ghkzaafmh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/giaohvpjz.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gmmgdprqa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gvykglydg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gqhtgpjim.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gcehnytsd.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/geotvscna.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gzpiapyrv.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/giuvwoimk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gpygykbpi.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/ghmewwqfz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gbhoawdad.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gyikxmrgc.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/grmkdmpyj.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gccthwuiu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gmfhlnzbb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gqbmcvszm.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/grlrwkmlt.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gollfnziy.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gnaxokrde.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gzjbkalqz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/ggkpvvtez.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gbxfvzfrv.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gbmyzhebf.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gruoscyvi.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gwnnmjtof.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gclswuhel.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gsijjgkcw.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/ggollqpcv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/grngvrrlw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcuwxoupe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gmqzwcbxb.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gqgegnybx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gyvsdmsar.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gnxjgrtmc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grtgqtkwy.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gcmrthloe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gxdinxtpe.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gmvohrezk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gcptxpamm.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gjclixmnv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gbifefwkw.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gjrahhcmq.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gbljpgykm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gzwsmmwfe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gvzcrboxo.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gjrkljjrl.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gijbmwskj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/ggtjinspt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/ggiopdrff.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gjwtsfcwl.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gunergbvz.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gpjbmlkjl.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gtgivedvi.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ghcvjvkxe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gqjmyfccl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/ggdxqcgig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/ghgvibrze.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gedjrlfer.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/ghrfrybtv.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gpqacumne.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gwdyowulx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/goyyamdlz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gbngjkrtr.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gdbkkibet.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/grvglcrjr.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gsxrgjota.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gfwbpqvfb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gexlsxxzw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gezxsmgcj.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gzlbsgtng.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gfujmecrk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/ggbzdnjbl.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gvisfbsqp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gdwiqgjjp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/givnytbui.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gerbidtgw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gflyuzitb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/ggvkhebfp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gmfafuqvr.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ggxjtcnau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gcdgdrbfr.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gqatcwvig.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gaqcmlxpd.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gedvsyxze.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gwpmkgitg.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/grslstgqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gyexmskzi.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gcbwmqcyn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gyirnupmd.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/galcfvzfc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbbglvzjg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gwodoyieg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ghzoxswkl.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/ghlxiwfqc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gjbqqrssz.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gjjjmgggc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gapdvknoh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/ghauofqlc.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/giavgsxef.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwjjsqach.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/goanqezbl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjivqjjqr.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gldpbbytx.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gajfaemab.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gwplweocf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gxdnetvdd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gigezofgd.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gsnunspht.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/goucvxoqq.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gpddahfcp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/ggqqcgbbi.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gmcijpcxf.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gpwfapynj.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gvwlpbzzw.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gikzrtatr.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gkybbsdub.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gyfgwpjbt.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gxtxujykl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gkmdhjznh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gchueywuj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gemxaanub.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gzuqghgvq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gidzcwalg.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gswvfjlgs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/geyfkevtr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gmmrpmceh.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gznjxbjoc.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gmmplqqqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gusguhyyp.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gvbkedgmr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gukvfaiay.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gzriqggac.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gbqncfblo.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gescckiuq.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gjsjhweoc.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gmqbxrjxu.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gvjdmxvmn.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gydoqbgme.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gqvoaouwm.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gpomntzql.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/geckppmmf.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/guvttkhzx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gtoqezndk.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/giapnjiov.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwmqwmkwo.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/glisjcyds.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gqmtqlffg.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gihiarkxc.sHtML


<!-- 参考信息 -->