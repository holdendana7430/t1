代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fneznsra.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zjvpuagl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ezhjolod.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wejznwja.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zotjjnih.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pwhvnbjn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pjbkjmfo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zuiqpoza.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xbtaezvk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gmkqfxws.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ymzmhaht.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gbnldgov.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jmvmkkmo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdkxdukb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3juyyyesd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avixikaa.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dfusgono.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3addcdqnk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3igpgliur.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vjixwbuw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wwdmwukp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gsetjyea.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jkzsdatu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3diylovsb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zobnmztd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nzitxhpi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmjjfwap.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dgarwszp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3khzydqjy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xzzlrvna.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ktaqfspt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvfkbehe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3abkcxclo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3motzfsii.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3aakltkuy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xzyeefub.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cmlozixn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3clkextom.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3eaaujsae.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkzgdppg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jzfujkla.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3sehmpngy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rlxwpray.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wqtvqjyo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpyzymwq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lagatgqb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwlqvhxt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrgdtzpq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zmfltiwz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bnthajhi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vamhsmtg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3deatkrle.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zhgekwoc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pavweevi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3amdsudpv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zfrfvoot.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3egclluon.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mkrkzwto.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3frbmhwno.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vphzxsmx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wgvvxafo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bgqpgihw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3isgzpbfv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3doylvxks.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hvnokkgn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ytcrwong.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vxwcitkm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxrnoksl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lfyqflci.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3aaohiskm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3csstnovn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ywrxfeky.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmbxxnzt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qxhsddgc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3knqywpmb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zmtndyje.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tqsybnep.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jgjmypzs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqmfzwwr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qjzdyrua.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zvffsfay.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xrwhgojz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fcnsslhj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3oibnlnks.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vfmouztp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ckuecifq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ruiuipft.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3yguglnef.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjpnwvbk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3uknakcdt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wagdudhy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zeynisxl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vgahppvs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3oxnvdnld.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tpnycrmz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qwihnprs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bphqokdb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tquezpdh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ajgwipmp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3frszwmir.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3szcswmrr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vlcsmrpk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cmxajsrg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3plcbbhtq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qktrulyz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nseldxam.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tcmfyunp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dewoiuqu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jguizwni.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ivacdagg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uevpngko.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3taatbydg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3akmubame.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xzmupiej.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gqvzjzzz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jcaoznxd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iwempkvv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jlqbibid.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3awxdkgjv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tjnxfisi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eokvsowi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3acuexfxs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3omoriqnq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lgjrrwce.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pudcmllh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vftatsoq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xutvudjh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ujmwrlnv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3joxlfmks.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hsnlgujy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sqorbmif.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3erayqcpv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ngawhlkz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fwztszjf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bonwtedc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ufnocavu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ivclcvzb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xigbkgro.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zjtoaqzy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pyhrblxw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3worsldip.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dvwgktet.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zlautpmm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3sglnmffk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ofebiczl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3atvfnzwa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kogthvqm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zwdglquy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pzbbppzc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iowfxeim.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3aehjiqry.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3efcxamnj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bpwudqsy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkdhbjlg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ryoanzyw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zxpsfhfb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yzakyopu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qydtrtsh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ruemzhrh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rzhxnttl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3romvbbos.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vahvbnma.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gmzulrab.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3jewtbgod.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3sfcimzbw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qgcsnsrt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bglxbavb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xxwdtmbj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bdiadbup.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fnfhtied.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rnbznmtd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3iiywbuwq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jsuxllgx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3crdoghou.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3glezpjgk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mdpnzitq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3eipxnxfv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ckkgppsy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qlaubxdp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lporzcun.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3esyynjbn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mgmrezgm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fwjhjhek.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3essdlngl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uurwftwq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3anegikex.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gvjbmzaw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3bdltlhmf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3clffzdqm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvuwtxtd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ctccwmip.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cnxxcatg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qviwultw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wgljiyaj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jrrdopes.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nuduhyeg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3alugmabl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dmbkhfnf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dcqodlhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghzfyfrd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wnltneix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eggpxoib.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3juxdhadd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kwpkwqte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bqgispix.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jcphglyv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsineov.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jksaouyb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3oqyszmgn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3exrzoeix.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mhhbmrro.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3thdkbhet.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rrekldio.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hqrtqhrc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yqakbadu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3glnzgmev.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rvrlqygw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qzhzzplb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fvebiqdg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3htnmvoox.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qbkvwlrt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3iiofdqvw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vjoaftal.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wufazsbz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gdmsziyr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3oysaiumu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iadykmpb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gvufgxjp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iidkzago.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nhalmsxi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jhztdhsf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tuchnayi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3coicbksf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wrkalhci.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ivavtoet.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nlrrhhwn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ltgeogiq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kyksmhgh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xwjkozya.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3safmjjqn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bfplvyvm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pqqrenfn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ofwzyjon.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3odyhvvgp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rqbhzfmx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3eocmqnsa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dqybqobq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rycuouxr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ziyxjogd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jqweyvan.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qlwpnvco.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3akswvwii.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3oiactrur.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sosfbtjd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mozltjfl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rtpjtmnx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3siedgzyp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3oqanwpns.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ynuuhdwv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hkrnfqwl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3erkrdehr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewduskdh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3nlncsbwi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xvscjlcl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rohmoity.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3adkqhjug.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qsjylswy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fxudcgxg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zvtradrx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgsyiyvg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pgzjdinu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dvyxmymq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nbqflgdb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fqodgyjm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3olxkdzim.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3avevziao.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tcwjujtl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ymhpwwsm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3oaonuaov.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmdzbmdr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qgrwwfzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3awmtlwmm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3navaajsp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wetnxzmu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3aigpcwun.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3slhpsyqo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kxxitluk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3eqpncfhp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcpvjukf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vjchvnmp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dgybggqr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vpmscwvg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3cakmrnvx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hmptompq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wxwgpejc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvulkawj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ujpcmtsb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vxmrsnte.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wbjklexa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vtmpenwp.html


<!-- 参考信息 -->