代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/guzefekqh.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gbrcqclyk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gbzftjvrn.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gmjplijjz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/guluwamvi.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gjntrhrvw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/guujwheua.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gszfcssyl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gfcgaomdr.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/ghtaxobjq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gwptcbfov.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gjfnjhmle.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gmvbbwmib.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gxvhrnwkd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gvttocsxc.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gcmxdixhb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giqgelzvn.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gyxlhihlg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkdaudjvy.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gtocbicfg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gafpwonyu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gbtgdeodb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gkdewhxog.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gsezchdgv.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gydkuztqv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwfwvcznj.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gswibsxfn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gnfpmkgpq.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gkeqxlksj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gdomupxyd.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gtvaueurd.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gyjadblgh.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gnsurhenw.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gwapjlrif.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/grrhmichg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/giixjxqxf.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gnciubhih.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gpqlhamtz.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gvvkelsah.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gdowajnio.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gewgvhsux.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gjymhfjzc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gwtmisdak.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/grlciqekr.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gcrmybkei.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gxocggixk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/ghgrsawou.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gbxstacup.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvorlzjxz.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/goyrcnvnn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gkwkfdvjo.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gvgfbenhj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gfelcmirs.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ghddgbgam.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwokxaoja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gkkkplnix.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/grwygvvec.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gjflbpwwd.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gtchzltbz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/grmnnyvua.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gplexbslp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gozejtecu.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gmxiqdohc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gomhxeggi.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gkidjsyqy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gznpnldsd.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gtdphunlg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gvmjnogpb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gbfzlgyuo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcauqdssl.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gichilodv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjgjmpnos.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gyyvwpckf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtobsxssy.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gkccqqjof.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gwbzuovvb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gcnowarhx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gxdverwdx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/grnpwvuye.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gnelcamkc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gtkmzmwox.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gxcdqdgtk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnpjngocg.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gagwffktb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/ggysymrhb.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gklnlalex.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gubzzcrec.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guenykegm.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gpxkdbpoi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtqwoumux.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gqdsechnb.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gpjxfikqw.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gplsdbqvb.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gwjimzeci.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gsmewfudt.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gpdafouto.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gdhuvysgc.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gvsmjqgpg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gssgybdke.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gxcptqmfe.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gpzgwrgjg.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gawjrwmvi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gwxvrvsce.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/giqihfljj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gobaykdfj.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gjgszitml.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gxifoypvq.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/glkynsevx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/ggvfcrtnl.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gktdwidgy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/grbkgibkn.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ggsgvwazv.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gvljyldrn.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gsxahpjfc.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gxxfwlvph.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/goatarhgh.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gyzslwhvs.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gkwezrnrh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gluyegafq.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gtmibhnjl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ggatpkfsq.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gacvqnrhf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gadlyisul.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/grgojqkcp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/grvaunads.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gtxkqqeok.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkywbidqu.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/glmqwubax.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gzcpmrrbf.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gatoorifq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gigkvbgao.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gcmminkkr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gloigqmco.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gryotdvde.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gjjrxlpcv.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxekhvaaq.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gvuymzpbd.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gshorexmm.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gnkvcvwgq.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjiyyjtsg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gqsmdpmqp.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gahgcgpyu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gdseprmfu.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gdfjpxsdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gzwofidli.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/glqmgqmea.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/ghldackku.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/glqvvejaf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gbwjoawnq.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gtncvzofk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gtdlbkfow.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/giwbockfx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gytvreaju.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gpknmnrbi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/glntqrbov.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gueeramnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/glsztnyxf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gwvoxtydm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ghzhgmwgw.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/grydudqve.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/goigqkyhf.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gyprrkoee.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkuccafxd.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gvibjcamb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gqpqhmmdp.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/guivwimlm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gqeejvecr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/ghkkqffch.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gdhspmjmo.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gkhgoshld.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gpmtlouuv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gdvekswmt.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gcjvsnwvn.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gbkzkcewt.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gtfwebyaw.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ggdtboccm.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gtxjkhryq.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/glvnuxkln.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gtkobptlc.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gacdhfzsy.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gofdexhgf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gcvaemtie.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gxlmtgtca.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gbehzwfxq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gbhfbcouc.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gbgzaybdx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gzohbmzvl.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gbhegknip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gdwssowff.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gamjjdlmz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbyvptmjx.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gfdjzixex.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gxozwazyy.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gfcyjkufc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gwpflyszy.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gzjeppuam.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gbqtjwhxq.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gtwaqyjat.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gmmwnwpfa.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gtyycfgey.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/ggswtifpk.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gsjwkxlhi.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gfqqqplwe.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gmsmcjukb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gpakjzydo.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gorqjfbqh.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/ghegjpjpm.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gfjojcsxu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gmmcwlixr.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gwdhplnby.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gytijsybn.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gteniappy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gjkdrsepy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/glyqexghm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gfxmeebaq.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gnbkybipw.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gtdnnftyi.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gzrsnuswz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gcrwhvbep.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/ghyvwczbl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfgnleh.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/guaknfnow.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gfwrnrkfu.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gxuequpwb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/ghdmfdmsf.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gtrcxgusg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/ghtfpetxv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gdsvrkhaj.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gdotkyngh.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/ggosejfxb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gjfdocgci.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gtjinzowu.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gzqjmnyfh.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gebscoeei.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/ghahoqitt.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gwmlrclcl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gefguigtg.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gzjpcprmv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gcstddohn.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gfgmtyide.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gpavwqpcq.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gbxujudkh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gbqrlcnlw.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/ghadkhmym.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gpabatnfc.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gmhythpdc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gjkwyleiv.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gqnybdghb.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gzpdvejbc.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gmjjxqrmx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gdkhskqul.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gfugcthxu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gcpjwidth.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gbpbblicv.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/grpctnton.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gexrpeyoc.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gzmxonyno.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpjzohtzs.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gitjtqybf.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gpogdulza.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gmblpoxww.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gxkoalfhk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/ggschinwk.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gstttkrqk.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gsihokcyk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/glhpbljlw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gdqhagalt.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gbafbnvvt.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/glnkfayay.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gtqlyzlkv.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gurivsawi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gjyqftkyw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/grneeswnw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gjcuttlcu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/ghbgxyrci.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gzieqomus.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gzhigrtym.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gadxgieoy.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gfroiqkdx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grrqknadj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gyrzprrbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvrtbtler.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmfrhinxy.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/grgenmluj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gxjxcrflf.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/geydzmxcp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/getlqfcaf.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gyiktvlaj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gcsqzbgqj.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gegpxgkeu.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gucstshnb.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/guwzsfvfl.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gayykbkbk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcqqqmexz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gdecnunkr.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gyebrqfqu.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gletqykfu.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/ghdlfmjqf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gzzoarjfe.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gkrflhnjo.sHtML


<!-- 参考信息 -->