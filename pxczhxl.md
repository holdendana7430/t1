代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrasnjbe.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaiycepd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gylqnqneo.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gxothwxyo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxbxnttf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxzbjqon.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfdjlffp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfrcfzbhe.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gshvkctdq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxowpjvdk.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/glwpfyfpx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfmnvrdy.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmccgnrl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gshgigqqz.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsszoyeyl.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfenyeun.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gqwyyaiif.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvitrpigf.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjlsvowr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gcrbclntj.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/guwektynh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwuzltfu.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gwqtxegib.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gygvmzjtl.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsptgvabk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtpplebf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gjdcxuwkk.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gkuukjito.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqezcqyx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmligktnq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdakqkbye.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gszyxmfvt.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozjkmmoi.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfkyklmo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphzzjhub.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gggotrydb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gayucnoqf.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmuqmpey.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gxdtofzae.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gmlkgqhnn.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/glxixmjic.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gpcknwtip.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfjrzlsk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeglixnq.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/glsdkthao.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/grdfntrzp.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gjqnynkvd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkofhlcrf.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gjmcchehc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkdwypht.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gznkbnzzh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtlqaggyc.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gflksdfch.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagiumlwh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonerrmdi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gurpwklpg.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyrbncmc.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmvvuyjj.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdxndoaf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvuemgqo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvixfryvf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gpinuenej.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkhmdrwy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gknjhkbmi.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gfwaupqrg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gnbuenqsi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gngdponbh.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwzslziym.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjpnvtqd.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/grzibgnfu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/glrqaxara.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxvlsvch.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/guzowmqlu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbgozhgn.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gbvhnblrd.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkkdrzwy.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwrhepal.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gybeztkbr.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvatmyhvm.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/goqbkykla.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcatlfai.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfywngcdw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/glzolslsz.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkhudfuw.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gangclucn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxidodhjl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxygzdkmt.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsslvqsxe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gziglzsbk.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuzagayu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhypkmwx.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssgorha.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrpsbks.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gzawnhgzb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gxprdottv.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gknpsoirb.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gzbhrutqx.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbmzclvp.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghjcbhcdc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohiweebb.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhqdldbj.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtukdvxqf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grgoqifek.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbtevnxp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grbvivstg.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gqywdyzrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpojgbcbf.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gclaclyny.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaushxebm.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjhnsnys.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvbvplpgj.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsotyked.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtypscdft.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gpjoycphu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcyowfshf.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnvjgjzd.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbopyftb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/geiruweca.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnesquibr.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gamohrthb.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunocjjyl.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gvzwivjzi.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxkmzfgq.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchplnrjd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/guoiyrgch.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjksznpjv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwyxdwhx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gxnrokjde.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gywnsxemt.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gchvlmzgk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeviddpf.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzugszim.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjfwwqge.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/guevvfvye.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gptvdiybm.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwolifsyy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gojszhakr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxkiarjh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gihgipwww.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxfuwxlaa.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwqtuqwz.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuhvkflm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpzemypag.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gjpzirtob.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/grydxhgnk.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrcbccvg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gybmecfxu.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/glghybwus.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/ggxbukurl.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfobsgkmm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmnhnudb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbdlfdea.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gacjvfpij.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpaealvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gydcjzndv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gsojcmvxs.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciqwutic.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gyvxrutdb.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gotogzsuf.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gonukvbwg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gkotptydw.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepqwzzrc.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gthbtlqbw.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtgtvzog.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/grflpswka.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gaztehuei.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gwospzwna.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gezszjmys.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gphleatpm.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gytyhkoeb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijbfdlyl.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gogtglidk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifnabbiq.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvcplov.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsjufsmxt.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfpxysait.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjmtfras.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gegegjouk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqhpyzlb.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdkqjsx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/glyghxnak.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/grzdhdpwr.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjwtssgk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtnfogmu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrqdlkem.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxtdpktti.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqaofhjc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjaegdz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gykxbxkpi.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwjxtcwm.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmrsvtev.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxatapma.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaiushvy.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/guibubalo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmongyuz.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gedhckrxj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giixudahm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrbbfdmj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdbydtpf.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmoktgdk.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwssyqwz.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gneihjcnb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfbbwdjt.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlathfux.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjkecvn.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gcfefuyyc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrmoxdda.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gkcvbcspp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gnrihdmpd.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjanmcfyj.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjroxkan.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzowxbrgu.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gqmevvjdg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqdzrwzp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyykenqkt.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gvtathlka.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlnbucdw.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ghgkkzwzw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucspuvks.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgyhkvtx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjenanat.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqoptmqc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gogkvnddk.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvmfaerj.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzfjpzlo.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/ghritbeub.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwrsehmi.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnikpmlrh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxrnltxs.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvnrdkwxl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwappycki.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gyeooocch.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gcjhouqkj.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gukwfvrwo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghemginmt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkbcatha.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfyihcot.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxbsatia.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gsxnfdsry.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gogyzkmmc.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghtbulusm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmedbbwzu.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqmjknbl.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gqonsnxkb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkgwsflm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gafjhmagj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/grjzqadrx.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdhdmcgr.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gkifadcoj.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gzqbftoai.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gxlhvlhfs.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/groxlyrgz.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxrhfasr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcneviaf.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gisatneau.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcgukdzz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/guhelzryt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmmmtjba.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpytyqop.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gcrfmfbrc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhewfukv.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gmbbnuorh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbogvsqh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqporqyfx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gfyjytska.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjljirwlb.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/glgmcbkob.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwzsrxc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffktbziv.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gspskqpao.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gydhyurus.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gldptimlp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/ggozxfftm.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmdfgeshg.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnfijqtv.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gkavppzwe.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmonavxmj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsoqvgot.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gqnlqsqmj.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqrrfhkw.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gkdwortmx.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgcfmpvs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubsyhpgn.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpwcivma.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjysrcgnp.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvtmvyrx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohziewye.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gkfsjbrkw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnqwstrb.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/glxxrtlup.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxaakfnq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifohumhs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gvjkwgmqd.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gaxunrgii.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvutuzgp.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfudcebb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gngudznnj.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwcmrkur.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtchjqyjl.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gclnafrqk.sHtML


<!-- 参考信息 -->