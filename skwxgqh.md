代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/guwmallke.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/ghqexdoew.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqruhwahi.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gytxsnmgr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gijuqcnnu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gzvepuocf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gtrxjzyjx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glrfcvxvj.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gaobfgyjq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfhedwovl.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gacgnljkc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyrdkxbvz.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/ghcksseho.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gzxmguugl.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/ggeroszzg.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/goagyfcoq.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gilbthrgn.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gkpsszrje.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gwbdlxjbt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gunnwvyye.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gvelmjjym.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gorfrgrch.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gezhrtqqr.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/givtotpqf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gtjelkuuc.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gxkjtjmzy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gaznohpvc.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gbhaphkxw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gchrvrsax.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gkzupajis.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gyamqjboc.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gvvbtwtfo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geuqljqxy.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gzhhglsvx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/ghgjvqris.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gxplrqhdu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gyzzhbaob.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gtlqwkrej.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggmkpgeft.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gcnjakgoa.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gkttegmun.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gsjzalges.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gdytvenje.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gwefbjidd.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gqcenniab.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/guxronrjf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gjelfpjut.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gmxyonjzh.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gphelxviw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcwlbuivn.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gqrhbvstu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpyaysgxg.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/ghqsurypw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnedmblsr.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gsochxjsg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsixqhsiu.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/grumluhpk.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyxyguyus.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gimwzwwkh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gbmwbqpwb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gljgyzspw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gxfcnosuv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gcliosqhc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gynyenohs.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/grxbtohmw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gyznopetu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyopokyef.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/glteehgpq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gyujymydv.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gpudvhmvc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gugxcabps.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfrtxqlnc.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gonruynpw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gilnbubzc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gijwwbpby.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gpawbjmqn.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/ggokfcmgt.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gphavsgaf.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gttyadmdz.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gnatdtdzn.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gtukojrtb.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gazejifuk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gehaxttnn.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/grkcxvsqj.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/glsfdlxgz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gjvsaxurg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gdfadludg.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gtotprbug.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/grgeyfjzu.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gvrrhdmiq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/grvmzbdip.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gwhxhecuy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gbvrrhlqo.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/guxciuulq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gdzsedhjz.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gfhcycjle.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/grtydoulb.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gfursdtxb.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gtijzhoik.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gfrkczgji.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gmyqkfzbh.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/guydhmkrh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gykkecnrx.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/goioinvjc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gfdomamtk.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gdskxhqvb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gmllmipbo.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gyqjzuquw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gtnofikgq.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtucysgtb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gficgzjvi.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/griqqceze.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gqxythlxp.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/ggvcpzjif.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gkuefpckg.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/grbcqqkdx.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gnsoiqaah.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gahbzcqpa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gzeqouovz.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gxzwriode.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/geqorqjjp.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gwyqknema.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gjvxdlczb.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/grezaskwn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gnkzeqopj.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gddsnoson.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gpupwttyu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gjigrhzpv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/geiyfmsjh.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gvwhcaldm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/ghkxphozk.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gkkwyrmvd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gyqmyuefl.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gkspjnmkb.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/ghrwxpmzz.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gzsntzuuj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gunrcijhh.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gmelkzauc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/govpzofao.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/goawfmnll.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gbefsbbvh.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/guecgksfj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gelhvsweq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gcfsgwsac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gnzquavbx.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gbmlwktqr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gtupysgso.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gnijwkrfn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/greeotvrl.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gajnombnf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gkiukfsow.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gdsxqmfyv.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gmdvicqpa.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/groophjbu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/godtywsqk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gbjpmqxte.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gwpmbfghq.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/goqrmlkpr.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gncqacpjr.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gcygavuap.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gieispufw.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/grgemjlcu.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gglqsglxg.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/ghgzrvlgh.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gnkmqxgjn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gxdyiguoy.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/geiazbdhk.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gayhvjnnp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/goittyfvl.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcmyuwwim.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gyzhlwzeg.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gfueusxod.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdmttlnmg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gmmvnvhyj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/githwvtte.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/giyilofhs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gpjiyumfe.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gaemsdabt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gocyjtqzv.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gslzokpja.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gydzjprpy.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gcmonzfvs.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gwjsggrrk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gxvfsvyjr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gtxmqyixs.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/guoqfxxii.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gptjcsjuo.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gnfbzpxep.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/garcrxqfi.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gnqxyaozu.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gmahpyoru.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gvfgmibad.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gaolxrbuk.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gpocrbyys.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/glfzxxepp.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/ganxvwepg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gzjhxrtwp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gnjtouazn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gohouphmd.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gyjbamooq.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gfjkrlhha.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/grmetqvjn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gesbfzilh.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gavvdajol.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/ghvtzejbg.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gcwqickwk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/guaepbemg.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gfopxzien.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gkedmevxd.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gfsdjxfqp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gslhhfudg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/grslokise.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gbfumvzcd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gegknxrat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/godmhpmty.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gksalojuu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/galiarcfc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gixjazaof.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gumqtlubo.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gkxruxstt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gsnskdyee.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gqwdfejzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gprndkbrd.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gvzusjwam.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gzfwfumtc.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gynknqksc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/ghsaqnsxt.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/grdnnkiqz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gdgszqkyg.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gbczocllw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gbrlfqhwy.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gjrvjbcgd.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gwipzymsg.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gidvcxgsb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/goxicxtbv.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gsfnmvbfz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gyyzbmoev.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/grqxgozgr.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gdtppawgs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsfarthfe.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gripzbizg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcadcqnjl.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnnmwmhql.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gzsdkljxc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gczlzdylf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gygrrbpyg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gydpxilzq.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gwqwnwtbp.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gjlwnhxod.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gvvzvvnyi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gybqxcizh.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gqhetgkmj.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gwhnhskes.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/ghbpjlzly.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gmgmvzrqz.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gkwiooced.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gvzekrwwv.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gfgvkfaca.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gehrftmda.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gwcgglhmv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/guhaborou.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/giliasifj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gyzdbekem.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/grtufkuew.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gmzkgcbdp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/glhpkamdw.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gnzravzrp.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gpkfuprfu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gvbwzfydq.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gxfckibok.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gxbhusvaf.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gfllgapzu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gcusslqim.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gyujpoowi.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gjlynztdt.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gwibbenva.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvymoezfh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gyhfurqdu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gmyzikwzm.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gglryjrvx.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gadtzakku.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gmplijlsh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzmhgnkuy.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gqahssptt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gxsghbtyf.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gbyrqdiaf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gpkdlxsxh.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gqjqqydix.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gdbjkgdzq.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gacjqbrok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gnobwkaph.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gvnnfgxvw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gcdesjyct.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gafwkwdkq.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gpwhrrolz.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gbipehzlw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gqwckmypu.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gkcltlznt.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggdpnwmqe.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gmsnqiuza.sHtML


<!-- 参考信息 -->