代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeecvuuo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkovqyupg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawthszus.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gptlqiljn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gghtkmqmh.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfydnqss.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/getiidpsy.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galuanmar.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxufhuvb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofopzcfn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnmcvhrh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gfiauzqer.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkzwahbb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvkoltbb.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gggnvdujq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvbwihzn.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/guqctjdma.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gsheiiumb.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gxhmlcuom.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gknmnddlk.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gewkcvjbx.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gghfxqxff.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxqpqljzj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gmkrnhbur.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gptkyjmoo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gliauhyby.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gjshiobif.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvbbiaszg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzdreoyz.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/geyfwxnaj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/goosismor.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gikckmccg.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfzwgmcsh.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gejvzjhpy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaguepdl.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpbvikep.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqutvvbz.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiemwxgs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gozoxyoqr.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gnrqsrvks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gfdrxxreq.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqyrwrzoz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbgpdybwb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gyhfjoezx.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gwuxqhkqn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gesgeplok.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gijgzygro.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyttuytxn.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geswxqiuh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/ggycznuwa.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbovzvcsy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gjebviptg.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gosuqeyvy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxfmmvfg.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgulukiq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnjthecvr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyawwuer.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gynmjxctl.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gayagwwct.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjvjlkgg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkhdlekp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godznxngv.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gniiynxnj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gswaompsa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gtpirmkpr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gvttxjljr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtgvigrfd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjpjyeba.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqplxeum.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gqitrrsfe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gioztvbqs.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gchvtkdja.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/grzexbbxg.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gvprjfeyt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzzuvtkx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfezosxc.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdazzhv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gznlggbbb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeomodld.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gresduwlo.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjrhadyl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxjjkkcy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaangjhug.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulmntmuj.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtitabwa.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbkwufrtd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrwbzzts.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gdlgxeeso.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gprmjfkef.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gepmzbalu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungbrcfs.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmiidsukl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqdaysym.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grtagwifj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsktwivpg.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjbtymsz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gyucfvjaf.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gwylkxsov.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaswulgez.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gitcilsun.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gaktxjnnk.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gpmrsygby.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gseocickq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjlgtpqj.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpcliqsv.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzfkbzht.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsvdeoqt.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpzmomfp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtafqrzlt.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gjyrzerao.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzkylamj.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwtvnphmw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyorrueap.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvafyfht.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnzbvzbk.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gbwsbvvqs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gglsjbizb.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gngdmoots.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gehzcgzcm.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkiiidjj.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwksogwle.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxaemani.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gthwhdaaa.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmubdrhvw.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdbuyodw.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gevvawfxx.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzedduqq.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmqinggr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtofsnttn.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqoqvyqh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gobvhjgfi.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/ghbxpzhhg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gznvxqjgx.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmjzbgzfw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gdpnhzitp.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfidhxrkd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzymipnme.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gnlzurici.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvkxktah.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdmszpeny.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggxsozeqp.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/guuxeqkhv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gasjbyiqx.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtclcjpbs.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gabvxtyzi.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/govpgbzrg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqgiubml.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjaxblouy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gdocatgnn.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiuswahf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gnrkpslym.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdqpychw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqxxhqu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbbjbcss.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgthaymw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwedkinju.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grxglhmnd.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gyplcmicy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/ggosyuclq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfffqfnbv.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqclvxntf.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkhtbfbgb.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gmjzjbfhe.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gebuaounb.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gvcjngkpt.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/golhkbivu.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpadpxce.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzsavspdw.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpoofyjh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyxaizsf.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gejupxiuy.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhyduvqt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlejyttc.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjuwclua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdjrxzab.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcmelmcog.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjoeqfnkx.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsojpcba.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdcoutviw.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gavbkeljx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gyjpuoalq.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/guosgjhmo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnzljalhp.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaczngtn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/galefhlmb.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gxddnyjwd.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsbhjocb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhcumjhx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadrhyzaf.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbctlaphi.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giwkrltxd.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gonjfaarr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gqflmizqk.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzldtjnqe.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gbagqlopa.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gjukiwuxw.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gqygdiqvy.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gntvwrcgv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gfmffhyte.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gnmuwxawp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gjmrxwywy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbqyjxpik.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gpkblvstg.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/grsdohyol.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/glddvzoyn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grbwaibfr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gzghueqwv.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggarkataz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gtiwbxton.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/grswybggq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/grvcughvb.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gajyggdfz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gteaeczkb.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtopawbe.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gitiqzyru.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzhjvvby.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/geqclbslh.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ghbuucfiq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsjyacys.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnmwtgya.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gzaxvjedi.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggczldggh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjvbzrwg.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkbkrdsz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gsnntzclu.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/grfighauy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsnskkqsc.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxtneggv.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/guqbvfbse.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwrdmjtg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtwfkgzeq.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gikgqitok.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gfyeohoyt.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrmymcc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/genhxujab.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gcotoneic.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gvvqmmnhk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbenaygyp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gechetlii.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgeylnbr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfabqmmsf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdogwotq.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdkmoiop.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grcdljdok.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gepljhgdp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfmqtqsk.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvgrcqdb.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrkluynd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggsnjbhvv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gelcrgpod.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybxyrbah.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gryjnycnx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/guppagakh.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/glyajfvij.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gnywsyxbs.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdweifrie.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuotqdbs.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfdaivlj.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvhuvfovv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvlrpgrw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gpeenfeey.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gbhcgfrmd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdznagtxl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqovhffcs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gktxtefih.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpysgzgx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijdqvtql.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/garzbzdli.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gnrrmpypd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gssduxnrf.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjwlgbtl.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmifgcetk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhnbkpuf.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghsabwtwq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/giqcxjaoo.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqrtohqpi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxiocvyz.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gkbgncmkh.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggrlnkaet.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrpncfzr.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdaumltb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvgcsxrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrnlqjxa.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grgrkklyh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnbpmyjt.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gobsyexca.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gfjflstai.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfjzkxnhf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniexptyh.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtqvzngy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gyduasgeq.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvmbncca.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gklbmwymq.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghriucnnk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpozvncng.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggpilrgyt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzgjmdpk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqccqhdvt.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaynedqb.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkvmdoyh.sHtML


<!-- 参考信息 -->