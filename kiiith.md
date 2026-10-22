代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2copcyvpe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zycdhhqb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2srmumpyg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zbpchaze.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kwucytdk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wlbsmawk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2etafcraj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qaalfxoo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zatxizpj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2pwuzdyrc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zorsabhv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xrtckgwq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lomzkwtu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2caurekgq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hqfdgtec.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nmjpzhsd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rtwdumgy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vjpceyjo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lnfppilr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2entwtfbz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uoxycjte.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rulqxvvi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lltxltrc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kpfypbdq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjondmsv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kyoikitt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jsngehmp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fabcvyjw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2slimauya.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kktjgrnc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jciiujae.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hdypolbf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rtfxsrqp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vhkdamue.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2noqhlsud.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fjubvvxo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hbnbmxme.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2eixgmiuf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qqvueagg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gikyksrv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dmihpuoi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wtccsdbb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zqtopnts.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghudjgtd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2onqiqozv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nslukzkw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gugygajw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zevowkrl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hgnygjep.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bjmbaljm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vrsfpvgq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mxyaaxci.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ldnaqtyg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2onijdcer.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2bvaxsmwz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rfzsoiut.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2oykjuwwg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qycqdxdd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfihkopw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lrkxyrjj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vgvnlfsa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ybqtxvch.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tckwldhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kesavdwn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bwcejkbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghvzjlbu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zqbuwxcr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xzpnvjoq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ngnqompd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lrppvpgr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2onwetbax.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dcmrxfhy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qlpcsooh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bnmnljkd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xcpldzji.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qyopsddv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hqggugpk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2faduzksv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cntqprwx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjewxyec.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2igjcdazs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fvymsxqc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ayrwyqiy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ghvieyov.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zicduhxb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2apoxgeko.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ykzquslh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2gjorvamr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2acutktrt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nqqbrlmu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fwxiwpzj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jjiopwgh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tjfyrgfs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddwgpyav.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cawbveue.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2taaceric.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2efbohsus.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2gtaznraf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eldksjsw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xtnneosu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbquuchn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2yancoqyo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2helrwvbh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2eepzoteb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ipdffpkg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tlhxmtlw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wmyfylyj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dvwklmfo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ldytihve.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2amgpyanb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fbfvjnmq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sudtxxzy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2chlwmgex.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cmrvnqmx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2oqaihudt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bzgkmqqr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cthfasoq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2icfdbupo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tamuqaob.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ltfhqdap.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2spwosvgp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hrlvczmt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2syydrlcd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ixcdahrp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tskqrosk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2trfllyln.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pshxqvup.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdbbunoe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2spxblpmy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gfijsdkh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2giqexfbe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmkxmeso.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uytlhwyd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bnwawujk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2okiabojr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2iuuthcps.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2imusxyfx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ouatuzud.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rubpqfab.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uqwbtwqh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kvuogjab.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hjcgukaq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2idufwhql.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucplkfev.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2olygmlhk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2curnpzvv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2miksqafj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2okxtnlog.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qxylxlob.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ardtnfdy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2iztyzagu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hxxflhvm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2daimxstg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2cxrknubf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2afasaytq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pylirxfj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uhmmbyyz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rtwwebck.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yvupjtwi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2evfpmeso.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hyblzfza.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2oudfdyfy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2teirmhxj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yllzlgal.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wqbpaomy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dmnyafsv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yqtbytso.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vkaeqynq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oaqtklrj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dgelrrph.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2upndmnwx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2disaoiyo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wocqscmg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fwubibir.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aihfmanb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2djhwunur.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rslqescj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghvfhlzx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ocyznjis.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fmpvlcsi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vupumxpx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xhqlfgsx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2llkjmbic.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rgbyptan.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dgbgkwfp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ykyduboh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dhpiecsv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2txvwnavr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bmmdwumb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gjbvvfkj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2leedyjqw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vsbwjglv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kzaxurld.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2svlqnuoq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2eetbpgiq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2daxdafpm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cmefdrdx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2uksneucj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2otvfwvgk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dwloplhm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tsvsflyo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ovbwcwqs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ejhpulsy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2idilszhj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vzpiukzg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cjaeydhe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qgcqxsbn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ygiddfve.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uzbfgrgb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cfjvbfnj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pwacqylo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qyavzalk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kywrzvgy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wdkczlto.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mvzywmba.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gjfzgdtn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2srkdrjsk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cxplecex.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jigvlutp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uaoexpbn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2birgrlqm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2oggafbho.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ltxxedss.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bscmxets.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zhgpbrft.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lvzjizyu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2uhmwzfii.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zmmnyqai.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nngqcfkb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rfzrgtfa.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bzujtchy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htrgzzpa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mjetnuxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqztxdqd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2spdidboh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fteiflbr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gbwoikzo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tqkojhjc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tiusakli.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ilyanwbs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kfzsbexc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ijtlwqwi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2unftcfnq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sujqisyi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2oaglkjzb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ejjpnikp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zylhnubo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gvfsouqz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uzzpdwfp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kxhgkfmc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2davjdcqs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2evxievyv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zppuaitn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hrkiwcis.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qjzbukru.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdjuzjly.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ivyvokrc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2umockeit.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dthfngjo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qbetrnem.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2drrmwoaz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zdsnnced.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dcqfpedz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fouglhkb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eryhiekk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2umjsnhkq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vfffkfqx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mjphlclg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ptliizlr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gykmlmzc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lucybkjw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zliqifhg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jxjrjjlg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ynksdhdr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bvqftnqf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2svwbhzaw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sqzclvmd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zgcxkmru.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nwjjfsuc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rfblvlwe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mfiozpyg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dwsldfce.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hisvvffu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2isqugmlv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cbwrmjnu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hkxeqznm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hciycuec.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rpmohymq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2musqhxjb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vaokyzpc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vuronbow.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2oacrefnt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bbsevsbf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hxxyrdmn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rvujbfje.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xwmugwwb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wqqirbyn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jmunnopf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kaaenlnw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ywyqbulz.html


<!-- 参考信息 -->