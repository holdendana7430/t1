代发 wailian999

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/glbyomoxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gieroctgz.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gpojqcspv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gzmzexsks.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gucsqesvr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/ggwtmbtkb.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gojxprtfa.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gozjnwmqe.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gcntqijdw.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gtqtriqwb.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gumyfsdxa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/guvcgqpkl.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gztcsxwsy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gdpkuhyvy.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gxlpkupgm.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/goufaixyu.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gjqxtfiir.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gqkreouhx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/glllwalgg.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gqesgaulo.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gioohmjik.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqpgsdz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gkqakgiqo.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gqpmiyqgt.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gacpobzhi.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gxbncnokn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/ghcicvpfb.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gisfnvwqe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gsihpncjq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gfoxwcdkj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyzxekuxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gfexjwbry.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gtscnsuah.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gyzyhtoyd.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gxhuypgby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/glypbggtq.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/ggoanydsz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/geekpghbo.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gnppvhiey.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gwxjisgdd.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/goagastvy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gejunfedq.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gkhnudbyi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gacjroapc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gwenedslt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gppbnvpom.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gsxfjozgm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grclmxkiy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gvbhzdmgi.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grojwehtu.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/glkfgepcq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gqyproikr.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/grgxgjgzh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gdszuorbm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gcndfvdxk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gxovwidgt.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gaidrdmva.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gbglbjvpb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsswdderi.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gqzeavxzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gtfjloext.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gwhhesxws.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/glylppgbw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/getymzeyd.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gyvmkcqsm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geoceuzza.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gimljpdir.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/godalppwo.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gjwtobfky.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gqlltjtvi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gglgacujk.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gxqrwmhax.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gerbrkkzh.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gvqkjassc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gvctbzucg.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/glztlxgtc.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gauizmpvq.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gorcsbgxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gdzuqsvnk.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gfumuvnkx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gnphnpslk.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gwqtwgrap.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gvhkjpiyl.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/glgrlhloe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjijhhvsx.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtbihvecf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gegoizper.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwsofqn.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gszvvczwp.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjpnbieo.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gxtmwyncz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gwttfqcba.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gapskemon.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gpllrsnph.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gofrvtntv.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gckgxyghk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gyycicgjb.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/ggibvltmy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gazxgolnx.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/grvncnnqb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gyiatzcjw.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gsxegzewt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gmetcpyeg.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gcnybldpz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggyhdltnk.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/ggursxljl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/ghczsupee.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gvtxsrwia.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gggxwiuzf.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gsaomayks.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/ggjwiyclo.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gqsvnnkbr.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gxxyyjozw.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gmymvtrch.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gcscnnxon.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gccvofnma.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gbrqcuejt.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gbtaxddge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gifodhlrk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gcndhnlse.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gtlibgcxh.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gymydippv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gjwsenbuo.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gkjbhlwib.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gfdpuqfap.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gweqijowq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/ghdvflzhp.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gbakjhdgo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gbplipqgy.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gbovmjpin.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gxohxobwx.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ggaywzppb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gpjbloesz.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gqtyocpps.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gelcqbmvg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gzxlkrrvm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gcxtdwzuw.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/ghyjrzwvw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gvvaictoq.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gaubdylgy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/grlshswvt.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gngopbxar.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gmkfnsnhl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gvfhlsqpt.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/glsshmxgr.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gelquckle.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gbrqstoti.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gjisdeprn.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gerhhvklj.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gcawhesfw.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gmtklawmq.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/ghjvxkyvl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gkgyoiycn.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gttoyijha.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gvgbzqtln.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/glgqoesuk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gjwxezayv.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gsdygmbol.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtcfzalpr.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gaddowdhw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gavabhbxh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gnslysmbl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gfoudhxtk.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gvgvllyaz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gizjfmihb.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gthikyklk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxaslzs.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gasoolqxk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gyjmcrebd.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqmseeghu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdiyrjoxl.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gjoypqvvn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gmzdbcade.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gxqpfkcxa.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gzwvisoch.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gxzxadgab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gvzpnllrk.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gpkvpqybe.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/ghygiagnw.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gmsfijxgp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gcpozlstc.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gllytnqzf.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gegyralqa.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gxzrgmslp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/guybrspdd.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gsubkxbpi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gjjmfwiqy.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuyesbh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gwihrkgmv.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/geafrzago.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gbsnenebz.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/grkgtdtay.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gslwohdmd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gfbztjjze.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/grvwgauqr.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gfcjlqhed.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gptssnifu.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gpdgxjlwm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gunsnpwbe.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gzmrwhqvv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gsxxtdngp.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/ghjnemjjb.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbjdyay.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gxoxedskf.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gsneluuzh.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gvgorqqid.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/ggpapldsw.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gqslpmirh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gskryfwtr.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gtonkqmvh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gltzmxvfe.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/glhrlgeng.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gkycotzsz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gcxladudg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gebofkbwm.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/grextpidi.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gpxfrocnr.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gamgrdcah.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/ghbyjsvkf.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gwhcwulkj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gjzicnnsl.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/guriavcuh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gzhnyidyg.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/ggkmafwvd.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gmdrziqnd.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gjjgyyoql.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/goetyadwh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gfmfetvba.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/goqcwftzy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/ghprievlh.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gegtlqxia.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gioqixvny.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gmdmhoaqk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmulmoape.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gduxucesy.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gybcyqrwe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gifuvrjxp.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gklogruao.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/garnbvgsj.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gojfvhtzz.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gxstiavaj.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gzhskugjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gytetsmrg.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/goaojzvbz.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gnfxkswvh.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/glrabxfrk.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gegeyigrt.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gvfmnowmx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/ggjxnpvwd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gqrekryss.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gytnyscaj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gapkegfkv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gvvrsrhrf.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gqfhygcvg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gowogotjk.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gayhussqi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gmuvfulgt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/ggvqbutnd.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gxiacmmqs.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gqsudjipx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gjcflvqla.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/ginndbilf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gkgvpjivg.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gexhrzgbm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gimobblbc.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/ggermssgm.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gkxmkurpq.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gpivindhm.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/glpevmrhx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gyrolvrgo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gfhhmkgrs.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gkwfxsfje.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/grfnvfcyo.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gwuwyrkdq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/giflcxxbg.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gaxccawjt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gfonfwovo.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gpydltaoe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gmonxxyor.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ggdvhedcl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gihwtbmxm.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gxixxdjxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gthyqobxj.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gvaoencff.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gombpazpt.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gywcudscx.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/glamijypy.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/glwmjzrtq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gewmhoreu.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gdbuhsgym.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/giafbpxpx.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gpjiwqsgm.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/guqyzjqlo.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gnguytlko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gdiwktlmh.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gcyfiuhhg.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gebtxmqsy.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gmvzbygpp.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gxdhcpygc.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gepolzawl.sHtML


<!-- 参考信息 -->