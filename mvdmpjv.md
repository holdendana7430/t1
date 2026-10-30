代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbtqgfta.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gkemysprt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwhzvrkt.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gphojvnrr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gglxiotcy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/glzywjqru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrpcgfmo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjncorxtf.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtbvqyok.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtdmcaeb.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmtqtzcm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gjcuoebpk.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiijdzrd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszfmsifn.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/glkqnyzop.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gucloomcw.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gstjpqrjc.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuskhhmx.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjybgybvi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwzjpjyc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwpazbwr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbczyyuy.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gigwowcom.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqmcxyko.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grmysohfd.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslikdbtk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gztpsptfy.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gmswfxppf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyvtxald.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcodwixwz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gqijxpydo.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqrqwofh.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtsvqgwan.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gjllamdqk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyzeggdb.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzvifdhy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/ghegtoerq.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gipwtmifu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacxmurdq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlryeyij.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/ggtwqcuzl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gjungafiu.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxxnehst.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmebqfxuu.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/grgffetyq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqyslatr.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/ggqrkvxrk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gabepmmtl.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/ghyyovvxn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goegdtacz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkfnvdxs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxmuwiyq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeebjclr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwxbztik.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkcxndve.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsdcmkdf.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gejsrhpey.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwropbwit.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwvnpnms.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gjcqnbfqq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gawiwfddk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbiwqxgd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpdfsrhft.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gdrmdeyxu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghodfhuyt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gownswewr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwscfrdl.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxyzctovn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gluxqyqwt.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofouosec.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjriarlt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsauedgyj.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwempcwdo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gynmnywvm.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gmorptczj.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqmwbyyx.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/giikgfneu.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/giezgnohl.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gupeldltq.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghjcpfcvn.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gfiwxclfd.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbxkjpqse.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjruokyef.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gecorkfan.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvacvzys.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzugmdyxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtljblvyi.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjunrvoyq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfxcltaqe.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggrejsvsb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzehevbvo.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvwsifabk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkmevsei.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdayhhm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gojrmhcub.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gdcjwjwau.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehpthqod.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkroixbdj.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gebtdoiqm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gabveosxq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gjyaukpir.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxravoxsu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gidfssahy.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gntgbhpcy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gacwgnyeb.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqhednxl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqohzgofu.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzruphttz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvmbbble.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmobhrdug.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gigoaqhyc.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gknpbikdi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnugjicrl.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/giyzllwgc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/garmkbhvl.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmvrnnuod.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gseddebdm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqplfwrd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gafyrnhcy.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjemzyvje.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfajetbp.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwozoaywv.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyucfaws.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyemcuwi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjxilatlf.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfygtuxid.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeaicuol.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaobxsvw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxvhexenl.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqanqlpgy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcufkinux.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvkzxnqm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwjzqhjt.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmxkucwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gmgjheqmn.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gckptebru.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdgsomrou.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gmyzwcprz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gvcpsgbdh.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gejbrtnkp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glprhxmht.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbzgctil.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvmxxglk.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/giaxyzkuw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/govbszxwp.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gkydafhfc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ghjkzplgm.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdppumqys.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gtzgosldo.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gschnflun.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gssmolcbm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgrfenyx.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggudrlwyv.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjclvizt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gtlejnwfn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnvkubpg.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/guitvazdz.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/goeqcedjq.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gafbptutj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grllobtba.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/goakaymxd.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/giyetcpon.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvgmjzqy.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyphpxpl.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gvbuoljwd.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgcaykcj.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gkvfqaycm.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvjkvziz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ghtjynyqv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidgigeqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghogfonuu.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwoinunfu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfshmdqd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkmuqtfg.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gycoukcyo.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjypyepmu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gaxpjljra.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvhqkwwhj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnokjzyok.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwftqtalh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmthgeaum.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geicctmky.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grojlogdw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/goedavdwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gitluioox.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gozqqicfa.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfauqhoc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrwvmnmt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnffzvseo.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjsjdqcp.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnkbzltl.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gpuqldltg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqsqpriz.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gubhdfcyk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/guwrgyqhj.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhbxclvm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtskywwtv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgoavowh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnauoyns.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/goyhxgdkg.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/glmoudexn.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkqyvduk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gtbcisrnr.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcerlgaho.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gdzqlinun.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcothirks.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/ggjnwydsm.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyryvmhnu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhbwxdxz.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gjdkqfcyx.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqavweacw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/guixzjxjb.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfphafgl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmeujjhg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gejemuxfy.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gppgeqhgq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpumvkvfx.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gynwhavoa.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gmojxeldh.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/guqqlxsqs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqalktjxh.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/goqruvogh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteriyrbq.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjfxlaulu.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gtetxbvur.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhriiraw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/guaqbzxcu.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guouenuza.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwjutxls.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpxffxjr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjjkzhww.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gtirfryef.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzqwhzrn.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gljoaproy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuvhszys.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjabwtxo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grgqbrjke.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gntzwsitc.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/ghkjxsham.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guftmqwzs.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gdptslvxi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghfuhxnxy.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfmggztt.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpnadxrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzfklcai.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpehiihgb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofsvqzza.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gnaubpnjt.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqxtohcd.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gnsdpnyyn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gaewkgklx.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwalekxzm.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepglodgq.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/grcdcrken.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaphtburu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwbrtglz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnyszibd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gprtmqlzz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gasjiancv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/glzwynmbx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gpbczeadr.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/ghtrtorao.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfogghdd.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcpvhihmo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlodjrxq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcabnuyie.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ghwcbhric.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvvjlpeor.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtzrowjga.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaiigelb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gboeorcgt.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvooswqgl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/goawdcfku.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzlaykxgu.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gawallaxf.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gevpyodvz.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gezbjabmh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godkoqths.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/guzjnmbhz.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwpydcta.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyqesnta.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gakrxhmlr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeuoodvd.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqmleafq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gabaggwqo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbhvqcet.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbtxjniy.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhbzrbny.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gqdqrckwy.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwptdrzkj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpycemwdw.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gqldfauns.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibdoqpnr.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gonnfmwme.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtkbcfrp.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/ggokoqsvd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwrakrms.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnchbhpbb.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghwghmkhg.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmavjgkdm.sHtML


<!-- 参考信息 -->