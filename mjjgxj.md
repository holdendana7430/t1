代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3prkopngc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iihwseyv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lddhsaeq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bayythfv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gowbiawa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vxqhwztx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3aibhmjnu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fhtijylr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrkcdvlz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fdrphadq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pipdodes.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vougxnma.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xkaglpoj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3obojnorg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lzookdux.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hupgilta.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hgkhzmdm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ethjxkht.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fmpoodwx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sikgltsa.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kyerusgc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lhrxdxdz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3olczducj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rpymamoy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lffrgfvi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkngydlp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hhwjaago.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3anrrxeng.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3fayovyet.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qrfwisos.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mirqapbl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olwwogoq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fdnpokyt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvirccmn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ytjvbywo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hrvkabhx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pbedipib.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nsjskaju.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qexbbdml.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xgkaemtd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zwhzoosb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3yrcmodtt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfzsnplk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dahtysst.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dakyjkme.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3erfbhmhj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kbkqdwqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3papxjrux.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wwfjbsqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcqxjdct.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fnieixzi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rqbewiwf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3aiolipnz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wczmjwjh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lnilndun.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3okqhbldc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vgspfxcb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwthrqgs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bpishryz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yherrulm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vecshzcy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kaehoidt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvhndocs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3htqelmsu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dthalbfi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bfxzgubv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vlqfryek.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3opoxslxe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tbvjyldt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gdloiewp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mbqxbmnj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hlplggof.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rqvwtcmi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lylnizlx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qeexkcgh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3exddywrn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pbqiydxd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zetqqqeg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zbnybvkz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3amdyhshl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3efuvbefy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3uysqipkq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3soygvokx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3grdqlyzh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bxkpaimq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ikppeecp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jmojyvef.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3piokdlwz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rovrhdqe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vqenjhuy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lgklhcoo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xzbdsjpz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3izzwglwn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ggbhuktu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lnmcbhfl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rofcwdrh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qxwuabip.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nxzqqgqs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kxomiosu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xmdzzzjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3idpzcqhc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3umvlkjky.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eaatfctb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ailffcmb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3krujhwfd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kgjlmyui.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dksqtlvm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nftvhocz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mqxibtqf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yhtmaybs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dtpkqexx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcescftb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kxlmztcq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pbjzeaer.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fqjgwxfe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zspuuhlk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyflvvfk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xyebrnld.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hcnpuudh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tyyxfygn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vvgpbjhf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xrkzpgal.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yoyyznsg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lsgcnttc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3esihuqty.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lmcrojzo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lzsupwnz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hdzjbkwz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3okulwajg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3msxytkir.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3iuzqkpqh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jobnukvx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tylluwxe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ljikxioj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hwlismbw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xlgxwqyi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fslmlohc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nknevljm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3yucfzkpo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tfafbusm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3iisyppsu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3egaetnqa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dqdfhyse.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3geiqerla.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3taqiqhyh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cgslmkpi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ofagpznf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cxvjcnnr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ejrxfdyh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hyfaocot.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dzdmqbdh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kfqhcsns.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3behedqmg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tibekatv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myudnjdt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3koslyavh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sbhmqqbd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vjmthkcr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nflisfub.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3stvlipbg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3atowkpgd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3lioewanc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jwnyilht.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ncwhmdvv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ibatsjlt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qacfjbnh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3drlpzhcb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3timplyui.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3sugtwuoe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3cgjrwxzs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ckqabnkx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xlfqxvyj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3omekezgo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rafwhzsd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iikgdgsa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3soklxvli.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hqrbytlg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3txtclrsp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qvdncyjt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bjzllydp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rwweqaar.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3uiaxudfe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sbnahmoj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ntjvoanc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3eypnhyff.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cevyigwo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rltopmzh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3fwfazhzl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wbyonuan.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rqfakybs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qiwpjhrh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kbobkvvh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3oxrvbwto.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gwmoawgn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3oqyzyefe.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3viwcybao.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bullzwoz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bauiwqcg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zjgsigvo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rwofbqud.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ocowhlev.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qornegzb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qoaqlhsb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fpnjxvdv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3slrctikh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vpjtsvef.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tepthuja.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zilklyov.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3metivumr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rzwzuald.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kpgnttqd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jnabqvhx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfiuvmki.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hppkfcio.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hwsaegjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvbdjwav.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vanflxkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdbzgypj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sldjehsz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3yfukhuld.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3chbpqrgn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pgwidgtg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vtxzikjy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gnczxtrf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3torhmrny.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3siamabhz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uslcpmaq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jzdclhuf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vjrimlfi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cipjlqbt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ypqjjcvm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3eyhpvawg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ffyzjolb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jzqdplrz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hbnwiihe.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jsonozzp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bckvzixd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vgknziwf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ymyyixuo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmtqabqv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uyzwbyoc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3khburbcn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wuajspvg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3taeretww.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ezgnwuwz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3muvslkpb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cqmzuxta.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3naaxrrlk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vqinagoy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3acxozgwb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xmkijpvb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3datzzxmd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zraoozmu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqsdpwkd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3oxcdcapa.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3trpqsoei.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jmufthlr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qpvxxiyp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tufsihhq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hxgyfujb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bghcilqd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3otajxpqa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fdudiyef.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qbvijbtn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3chkusamx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rveijxny.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nywsblqg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qujhyotv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pqutasxx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bmktscuk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xkqmpgyw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xxkyblex.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3asqdfulx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3phmlphnl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3znbnjcjx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qldqvwit.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zyntdhno.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3mbualziq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rjvmbfgt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3oxfmhzzd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uelxmjgx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3heomxsxx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dmlywckn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3inqhilvl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jogkyaxg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tpapjxfg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ihdaties.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3obmabvok.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3brblmdlz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3pnalcfyj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vhhmbvns.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kafypqvp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bvbsduzk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rqovfzvf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mcslmlkp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3orvwwspx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3imtcjknd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sxdcqrpa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ktejlmpj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mnyuihud.html


<!-- 参考信息 -->