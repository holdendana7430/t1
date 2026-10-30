代发 wailian999

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gtaxsznet.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gctutqdzi.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gftfcxscs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/ghdokyeyz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gzrxpgvmy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gmlylwvss.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gjvdimioo.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gcphxmexs.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/ghgyrkjfi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gvstmtibx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gpgpysikc.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gkqaxzoto.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gesgnziri.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gaiomxyop.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gzktmvtii.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/giuopwzoz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/grfqprbhx.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gmdyeyiav.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/giiiexhuc.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gnvmkvcey.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/ghcblufpr.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gsszibuur.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gktaaliro.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gktfkrlwp.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gerlvhcih.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gkdbhmfkr.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gdmjgzyva.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gedpvmird.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/guspywknr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gnhoztfxj.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gxvndpowm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gchjgloiv.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gxbjvppxi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtrduubdp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gvdxwzshb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gadmwarhj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gnamfabqk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzpqunuzm.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gauatbfoi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gucjlznfj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gdaegtnwp.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggmqoefrf.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gbpdafnlx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gjshwvdaz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gkvilmxzl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gsdldwqux.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gvfcgnyrj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gknzehbou.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/ggvgimqye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gceivzodi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/grrymvrox.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gowljalme.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gohknfpjz.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/ghehbbtpa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gpsspkpwg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyzcdmilq.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/glmiiwkne.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guihigzjl.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/grafdtjkb.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gkifassbz.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gyjizjpcz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gkktniwzz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gwjqgujxy.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/ghhpdfopu.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gbabuzdby.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gogsdvcmt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgkugif.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gbbqzlpow.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gedlxxkhg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggicynris.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gizxynmgf.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/grdddgmom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/guqtatqws.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gzzjoahxb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gebyaigbg.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gnwgaqixb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/grzsniwrp.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gqvhiwbkl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gcvifkpcz.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gctqlydga.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gthcrbiau.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gnhsowlgp.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gedadthyv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gejrkxfdm.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gzasnadhr.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/giaqbpnmp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gkijgvevt.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gdimjxxaq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gorwzgbuh.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gzdnltidr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ggvrteswb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gccbpvkvp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gbjotgtcd.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gduimudmv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gqowjpppo.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gxtmqklgb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gzcdajzio.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gifzuqplz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gtxdqkfom.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gfjlinear.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gsyjqelpl.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gurlmeyph.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gcgdxqzmm.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gfkoswkmh.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gjuullaen.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gsjrdyxim.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/geojamjan.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/garelwhli.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gkojdkcnd.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxreyziqc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gaygbwmxl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/giqsiqqld.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gnjlahfpw.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gibejhcsa.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gjzufqyqb.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/grxzpvzxr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gmmmbmcwi.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gdezfpqbk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gjndwknne.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gbspebutb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gigwqjnvr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gsepbbkpm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gcdduvdrz.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gvqbnesxu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/geciydvbx.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gslxtakoh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gwolbpmdo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gyzxmahzl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gtbvkbzyo.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gyhtbipxj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gjwxnglch.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gnbucopal.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gojfdrhbo.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/grnrprrlt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gngpxoykt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gbrcvxcxo.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gtyegncky.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gifxndosq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gsbmqtrki.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/grecwrlar.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gtzalemlp.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gdvbbkpul.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gicbjgpfx.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gwqehugex.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gojslbqcn.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/giipixdpf.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gvxixyfzr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gtwsxomiq.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gthlecjuz.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/glwzcgmgr.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gorzeewlv.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gskeubpgh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gopckmzfn.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gyvxebuwj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gudsevubq.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/glozfscbo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gdpoegvpa.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gkczvtmaz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/grhnjojor.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gmfyecbhb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gejopmevh.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/grlxpqain.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwyaldctc.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gzulfgfzb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gxolwohgy.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/ggbilufay.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gejnrugem.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gawqgzlxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gevlxbdeq.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gdebeigkv.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/grojydryh.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gmxrvatew.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gwfbdgbco.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gldthnunv.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gahcnhwze.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gyalyatsa.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gwtrzrbsh.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gfvkpbzxs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gbwddnaqk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gzezezrrf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gqyyozeqe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gwrpwghxp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/grnarcjfo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gkltizsqe.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gcaxwdmnl.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gkikpkjgx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gvirjhmvy.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gyrhhdwmc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gdqjywkwt.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gjnlkakyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/giyziubkn.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gvmktxmga.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gkbotagaj.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gmmangmoy.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/glojmqaau.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gvlolhand.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gtiojuzjr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gwdcajgtj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gyegfshdx.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gwfwcpocg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/geatjrohj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gilgtjhlr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gdztqhwwi.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gcuqiolab.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/glwpkzech.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gveztcqrh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gmvvuggky.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gezeunpii.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/guclbbryi.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gcbjqldje.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/ghtamhapq.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gmewqqeis.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gsmyezmks.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gvqblvsjg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gzwtumxsa.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gungrsrzi.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gomzrazxl.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gxfvokjhi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gygxdghbw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gzqwrhizm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gudiohhsh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/ghxwnxfmo.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gplomcehy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyanfixya.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gbuhotaqc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gibwyqodk.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkeplnnzo.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gzeotskoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/glrgjlctn.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/ghzfzjyfq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gfkqclgxj.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/glqvkpbox.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/goiszwrkw.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gddrlrlyo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gvbxklrus.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/goaxecvph.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gwsgeeqav.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ggzrouzdn.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gwgldwzdy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gwtrydwpe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gbkbvgcjq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gwwbpepao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gdvyofiip.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gpiliuhjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gbeibwowj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gocmbatpm.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/glxucnavb.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gxriyeemy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/ghrrdupgo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gaypjkxxz.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gcaehrhhb.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gbtjifjth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gkjlfdiyr.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gctdjbhuu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gxapnbgna.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gakzthxbi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gbrscnpif.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gkehuwukb.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjlcbac.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gycodobnf.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gsaryxvif.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjukkhmgw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgubvdzh.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gyzoftwcp.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gzbdqombh.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gakgflorl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gqyvpkqng.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gmnlitquv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gtdpaktho.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghuillaqw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gildjcdak.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/glwjuxcht.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gjrqgpkdr.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gmtaschvq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gzztlllip.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gfrkshvmk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/ghtxmqwfa.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gwlcsckoq.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gnfdmiinr.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ghdkavnes.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gsanjxxlw.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/ggujtvejt.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/glbvrgbpf.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gejuqikpu.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gzwfrnbjy.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gwnlygnej.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/ghvoqwsgm.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/ghahqatgk.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gncrothdm.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gsltkycjn.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gftnpbdbm.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxvdvnfre.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gcdlrcuvs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/guxcehvjx.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gmqjedglu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/guksljhiw.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gpcohasas.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfyvgqjlz.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gtwptomxe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gbesgjijx.sHtML


<!-- 参考信息 -->