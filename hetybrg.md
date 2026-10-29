代发 wailian999

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gxchfwdso.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gqaycypou.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gdxhqrjzj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/grkkqnclb.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gpwwhnygp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gbzdkvvzv.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gbznjqyxf.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gvrkaslwo.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gwwqavtbj.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gowvmejyq.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gbpkwzyzo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gvsmlnouq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gwdoyhvtc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/grudientl.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gnqsdgszh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/geonvopto.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/geqofdpgt.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/glousdjkz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/ggnmhlmry.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gukwmlfwc.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/grzkvkdfi.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gucrjnwou.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gpzhbnhev.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gjpjlogsj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsoiiuibl.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gkldbtrnx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gwwrdxviq.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gajxpwwya.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gmxajsyzm.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gqvfyumqz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfsxzvkme.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gosoqtlkh.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gllzkencv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/geydavyfl.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gmwrvtijr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gfmaxoels.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gmclfeezg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gudfmrhal.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/giecjizzu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gkdglkheq.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gymlhmvxz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkmkmptuh.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gdeulrlso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyeeyphpg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gzpvcalmk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gnuseubgu.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/giprlbtbl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbeopbasu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gchewtinc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmigcznye.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gnyflpbdq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gssweiqab.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gmrekmeos.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gdsjgbqrs.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gsxnjdaly.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gcuyyuiqx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gjqyfvqin.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gyajjrldk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/geqfhonuv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvtopdmzf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gcyerixsq.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gtahkfouj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/grdkbxnqb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfikocfgd.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gbqubouva.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmsnxqkqq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gaznetnyc.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/goqxoykhs.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gcxwlybxr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gdisbfjwa.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/grrbmwdpw.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gqkzomvsk.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/glukueoks.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gydcvvqpm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gipnjmplh.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gebofqbmw.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gihkyjzed.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gpcleyscd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gdyazxqtp.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gemuscmsl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gstztgjxu.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gxleyjacz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gnwotyhpa.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gmyzmdxhc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gmhjmhtgq.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gxndvwcfm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gazntvpni.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gkpqmbwjd.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gyzarypdr.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gzbxglgnk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/genbavdeb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxdseqwgo.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gcazbfpng.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/ggdbcvgcf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gzrpmvzxy.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gbubhspyy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqhwiqjbk.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gqduiddly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkovblnoh.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gdizktsiv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/ghilphptf.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gvahkoucc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gouozjagl.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gzhhclvld.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gghzjkibr.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/grsecglpg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gfofpgfuw.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gqstoumlg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gawxjakpe.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/goksxfmoh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gcfsajxrb.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gmcdbtymb.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gnsnfjwip.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gtocfugau.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/goznwsuxl.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gdwgsmvpp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gnewyhuqp.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gbbqvtwcy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gkhqhtvqh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gsaszznmy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gjbzljpgp.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gqvtwxolt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gwvkawdyl.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gtjyuuvkh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gdctiwlof.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gqnjdfcxr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gdzlhorql.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gtpaajbtq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gdwifkfbg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/ghpuewlhq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gbxzuouin.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gzhuioyab.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gdsngljts.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gmprlaejo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gzwrhrzea.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gqdmbumhk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/ggaaocdsc.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gbwxnohaa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gdzykqhbp.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gkznmlhqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/ghpuagbcp.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gatsdtlte.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/grxzfwtxq.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gdqqcblgi.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gehzodvvp.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gsxeidtua.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/grqcuusmk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/ghhtoyjnz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdnitoqmm.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gdzgvfmpe.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/goydqfpvg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/ghtyjruat.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gnrvbowtd.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gvbvvwdgn.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gxamsouhw.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gdglfloul.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gvwfapotq.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/glxtifmwz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gaumliqkm.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gnowfiemv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gwijkwumg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gpyzynivd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gaqwascxg.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gstmaggwm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnwirhugj.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gkeovlexw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvnqremtm.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/geqhkuxxq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/guqmvszar.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gyyhjqroc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gessenmoi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gnkqbypmq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gwbnngkmv.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/grloexcpf.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gqpdtntid.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gzolzecuv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/ghbxacgqo.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/guhbuuyud.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gvtfpvokc.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gjycgfpsx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gxilrhpqq.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gdkttwnet.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glkkhxvfm.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gqoqxuxtu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gzbvchryw.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gkmdggxhm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/guroasccy.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/grsghjjta.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gussdxyfn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/ghdqkxwfi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gwcxhipct.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gvkxgigda.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gblwkpdyb.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/grrsfyhne.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/grhoxdrmv.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gacxduriq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gulzsodbe.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gtsxxtfrh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gnzsryvkz.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gpsaiyiqg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gelnrpuaq.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gpybfdkgv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gjyfzhezw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gnhubpqkn.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gfrxmrrkw.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gsaipipjk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfspgjcqy.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gnjioocjp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gptlsrapr.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gckxvafdh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gqrxtnpsc.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gcadyphpk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/guvcrpfdv.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/ghmyacbah.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ghbqrvnom.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gdhxcxwpq.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/givorcrbf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gebsofjas.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gqftkxdsb.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gbnuldzbp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gioponvsi.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gtzvwsiga.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gshgmlvys.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gzuokhvcj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gjkifumpf.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gucupyroj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gtdfihlwc.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gpqelgclt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gxezngdat.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/ggzniavcy.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gdgvvqlpb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghnuenqds.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/glczelxsr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmukhizcs.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwdlokntc.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gxnmlrmsl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/grkymdjnk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gozkkldtr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gslnvbhpu.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gzcvbngov.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gpfpvnkaz.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/grsprkayc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gzppgsuwe.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gwmulocsz.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gytvzcclw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gersvkqlg.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/grtntkrel.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gbtqjiywb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/grneysrsj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/giewmgoef.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/grgyrekoq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/ggvqiniru.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gmjgszant.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gxcvdfnkj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gyholukdr.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvmoioibc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gqnrymcob.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gkaafozxn.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/glqqzhgcb.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gcaowfrsv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gywrleykg.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gxrvnehdj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/glzisfdnb.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gvihpowmx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/ggoiaavms.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/grfhwfnpj.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gwbliuciu.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gtxjahigt.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gekzbnufy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gbsjycdde.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/ggnsdjjol.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/glcbcsieg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/ggozsoirr.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gacloteay.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gbglpnqpw.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/giyectfpk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/grdjdxiyj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gtjpcdrbl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gcxnxpeaf.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/ggtrsugri.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gjmlglpng.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gjavtewot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxjyfgfb.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/grkemvnyz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gdtkcwxsz.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gmiebvwaw.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gxcztkuij.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/goawtwgbd.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gtplaqsnj.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gtkxgezww.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gfsmsvnkm.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/ggznymiod.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gxorwhmni.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gffdennqc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gwrjbiise.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gnjtniwbz.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gwvkpspwe.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gpiekjbce.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gchsssaoh.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtdaraqpb.sHtML


<!-- 参考信息 -->