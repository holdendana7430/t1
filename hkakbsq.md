代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkidgnlec.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxrsjnrs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gukxeonrv.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gehxocteg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gymfworxh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndrkvuwo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gcdakbqgg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwjybsf.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzhjxpia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbseoubla.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloqonwpa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkaowukh.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydsrqzkf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbqtfyca.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtptaih.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gpafwcwsa.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gcdfjhece.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggozppagw.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gneqamnrm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcmrkpib.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/galtzylpt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gymcvnnxm.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgrcwgkq.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/geygzipkl.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfdchjxt.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdodhxsw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/ggcikbpnv.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gmzxpivhv.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/givzogfnl.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gzexwuzyd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gknfrswcy.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/garwqrmxa.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/geofstrck.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/ggeinuahk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqykogjtv.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gwrwpotlq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gxgdrqlow.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnbgkxybw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gscfrmgwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzagtoii.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/geisjakne.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbrravnq.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/ghkloctoy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gufrnhpkj.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyfkspng.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gglcjooac.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/guivlxiqu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gbenxrycl.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlluskwl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjrfafkh.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvndselt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqmcaiqp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxknshmjf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnnwxigf.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpextkvg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gehvzlqvm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gstzlfwwf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnxxzgmip.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gpwdcpuon.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gatpzqyzw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzbbhqto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfktmnksq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gzwsydxix.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gzxhimksg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gcsgmkulw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gizxqpahl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqddbvdu.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxpmtgffd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqrewydg.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwljrjftz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmgbfbqp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/griwjyblt.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpnzgvyl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgghlsry.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhlxngxq.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/ggvfzjzvq.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjrrqrzr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbkpqwye.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpgvjop.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcbsdpwt.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/grbjrnosm.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwkacdtx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwfmgbmt.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godybikqq.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gragelvjw.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gpebfhupg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gburoyleb.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgivnems.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/goshegyme.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxogcbya.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gglckbkji.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepjgxvzv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfgudgrsf.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfyeobi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxqmtosm.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggraziptj.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gurmtbiiy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiruuxxu.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gymhknarv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrpnuzqu.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gvixpmngp.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gapmnrmoa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gujjqldza.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwfbmdydx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmihrmhe.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gimioxshi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gklkxftgm.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmotdplzz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvangzzaw.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyubvjttc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjbjnxgwb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjcbmzbp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gafgjheqy.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gqbpzuzmv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfxjcsit.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeihrnlx.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtixjpvr.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/girybgcyo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gihvadezl.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfyplzai.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtapcwizr.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyowpcvli.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzdblzruq.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpstvhqyv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbballvnb.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggxlylijr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqzzobnhf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gouzbjmmv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gaorxzruk.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjxsjdwpk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gqdjtprsw.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/goigurjlw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsuptprr.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gxgtdptwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdntxgxg.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxkampwru.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbtltxja.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/grygljerq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gogxktooa.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvejduul.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyuivfhb.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswhnodvu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyjdjlqib.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gugzmkalr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gptmlyrvz.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnumzmvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gibvcwyaw.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gvowewbwj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/glrakdjie.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxzgaklt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gxysvemvm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gozyzruid.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkokpeyl.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gkunubgqj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdslotodd.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gsqqkkjnz.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuozjpzd.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnilaurfh.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyozowqa.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/glaclmdel.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdjeaps.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbnfgupv.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbvjsxris.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guvlzjpfq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyjrwyej.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdqbafsd.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/grjrbaiqs.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjkestjhy.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/grjphdmqr.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gqsmeykbi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/glpopjape.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grlosxkcm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvccdarha.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmklaofk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlagjepa.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gajfaczwp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gthmkokuy.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdndhpifz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcwzeucj.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gkkallmdd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpctatgxm.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gigahyeqt.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grgxxpdfa.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gktehbuuv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/geljadoid.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsfpfgsrq.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbqhmyidi.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gctlepvvs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqvankns.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxnbcydrt.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gphozabcy.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfivvnww.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlkgdoco.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzahjkchp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gaugmtzvy.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gxrhifwyr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqtwgaqf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmhxwjlu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqisupfz.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gbtpouicd.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdylljvdl.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gizwvuhes.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlkdctir.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gvkzrshrq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gtweksvix.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gklqxwxhz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gmlofthzd.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gwvvbyiea.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjxgwvit.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkshewaah.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gxaubcsvx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gwijnzxbl.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrdtkqry.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxorasquh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilrltoes.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gtqfqplwo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmwgvvlq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxyvxhum.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbiyjbaj.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gseeufeto.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gssyabuwk.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gauhrqypa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkfehnxrd.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/guyqbldhd.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gklyponew.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gfghqgzcz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkkbabqpy.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnnsclifc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gfxkoqvfl.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxeauabh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gocbxinxw.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsubctpg.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gisnpeqsf.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gxksfjxkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgymtauz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyotiwmry.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaobjbvyz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gbpologoy.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gipksqass.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjowhhr.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gavfazxfr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gugntpocc.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqgmixlbs.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlitsogo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgandron.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gceccbdnw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gkldmzqwf.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudlhfez.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvndqmxln.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gojbyggdb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsexuqzpg.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gigsgrrte.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhatwzlm.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grgsyzjsw.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gydviyjoi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqjszixd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gapvzyykm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gfspzmfal.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/glotzltxp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzyixqdd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrvqovib.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gpbdmbhmf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcszwppwa.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqxudaybr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gofdbwgzu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkhbkwtj.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gdzidtvcw.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gksfswfrb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gitkxznpp.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdktlhjgu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/githgjwcy.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjhcugmu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjriiqfz.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gksmrooap.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gooorvnyz.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/geytvsjfw.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfkdgchf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/girvwqxcm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaftmqrz.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gokrwnumo.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glippdfiy.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbkhyegma.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghivykpxm.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/grpyvyboa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrinjxjt.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrozgdfo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdncndenn.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ghutzhtpr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghirhjbsl.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gthnmipdx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/glftfirza.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/goemvwxqe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/glihzhjjw.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gcashkvmr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcefwgni.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsbnkhzw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkynvvgyz.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gatbzjjly.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfagmzcqo.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcebffpk.sHtML


<!-- 参考信息 -->